# Advanced IAM Access Patterns

OCI IAM supports different access patterns for users, administrators, applications, and cloud resources.
These patterns help support secure access without giving unnecessary permissions.

---

## Common Access Patterns

This repository covers the following access patterns:

- User access through groups and policies
- Compartment-based access control
- Dynamic group access for compute instances
- Instance principals for service authentication
- Resource principals for OCI services

---

## Instance Principals

Instance principals allow compute instances to access OCI services using the identity of the instance.
This avoids storing API keys on the server and helps improve security.

---

## Resource Principals

Resource principals allow supported OCI services to authenticate with other OCI services.
This pattern is commonly used when one OCI service needs controlled access to another service.

---

## Least Privilege Access

A good IAM design should follow least privilege.
This means users, groups, and services should receive only the permissions required for the task.

---

## What I Understood

My main understanding is that IAM access should be designed based on need.
For users, access should be managed through groups and policies. For workloads, access should be managed through dynamic groups, instance principals, or resource principals where applicable.
