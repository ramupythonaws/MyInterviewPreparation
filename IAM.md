# 🧠 How to Identify Policy Type by JSON Structure

| 🔍 **Clue in JSON**                                                                                                                   | 🎯 **Policy Type**                                  | 📝 **Description**                                                |
| ------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- | ----------------------------------------------------------------- |
| ✅ **No `Principal` field**<br>✅ Attached to user/role/group                                                                           | 🧍‍♂️ **Identity-based policy** (Permission policy) | Grants permissions to IAM identities (user, group, role)          |
| ✅ **Has `Principal` field**                                                                                                           | 🌐 **Resource-based policy**                        | Grants access to resources like S3, Lambda, SQS, etc.             |
| ✅ **Action is `sts:AssumeRole`**<br>✅ `Principal` is a service or user                                                                | 🔐 **Trust policy**                                 | Defines **who can assume** an IAM role                            |
| ✅ **Action includes AWS management actions** (like `s3:*`)<br>✅ Often contains `Condition` with `aws:TagKeys`, `aws:RequestTag`, etc. | 🔧 **ABAC policy** (Attribute-Based Access Control) | Uses **tags** to control access                                   |
| ✅ **Used in AWS Organizations**<br>✅ Applies at account/OU level                                                                      | 🏛️ **SCP (Service Control Policy)**                | Restricts what identities **can’t do**, even if allowed elsewhere |
| ✅ **For services like AWS Lake Formation, EKS, IAM Identity Center**                                                                  | 🔒 **RBAC policy** (Role-Based Access Control)      | Grants permissions based on **roles**, not just resources         |


## 🧍‍♂️ 1. Identity-Based Policy (Most common)

```json
{
  "Version": "2012-10-17",
  "Statement": [{
    "Effect": "Allow",
    "Action": "s3:ListBucket",
    "Resource": "arn:aws:s3:::my-bucket"
  }]
}
```
🔍 No Principal
✅ Attached to a user, group, or role
## 🌐 2. Resource-Based Policy
🔍 Has **"Principal"**
✅ Attached to resource (e.g., S3 bucket policy)
```json
{
  "Version": "2012-10-17",
  "Statement": [{
    "Effect": "Allow",
    "Principal": {
      "AWS": "arn:aws:iam::123456789012:user/ramu"
    },
    "Action": "s3:GetObject",
    "Resource": "arn:aws:s3:::my-bucket/*"
  }]
}
```

## 🔐 3. Trust Policy
```json
{
  "Version": "2012-10-17",
  "Statement": [{
    "Effect": "Allow",
    "Principal": {
      "Service": "ec2.amazonaws.com"
    },
    "Action": "sts:AssumeRole"
  }]
}
```
🔍 "Action": "sts:AssumeRole" = Trust policy
✅ Found inside role’s "Trust relationships" tab


## 🧾 4. ABAC Policy (Attribute-Based)
```json
{
  "Version": "2012-10-17",
  "Statement": [{
    "Effect": "Allow",
    "Action": "s3:PutObject",
    "Resource": "*",
    "Condition": {
      "StringEquals": {
        "aws:RequestTag/project": "MyProject"
      }
    }
  }]
}
```
🔍 Uses aws:RequestTag, aws:TagKeys, aws:PrincipalTag
✅ ABAC is identity-based + tag condition logic

## 🏛️ 5. SCP (Service Control Policy)
```json
{
  "Version": "2012-10-17",
  "Statement": [{
    "Effect": "Deny",
    "Action": "ec2:*",
    "Resource": "*"
  }]
}
```
🔍 No Principal, not attached to IAM identities

✅ Applied at AWS Organization account or OU level

## 🔑 6. RBAC (Role-Based)
Not a specific JSON structure — RBAC is implemented in:
IAM Identity Center (old AWS SSO)
Lake Formation, EKS, etc.
You assign users to roles, and those roles have permission sets.
