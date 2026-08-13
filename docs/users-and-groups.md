# Users and Groups

Users represent individual identities that can access the OCI Console, APIs, or CLI.

Groups are used to organize users who need similar access.

In OCI, permissions are usually assigned to groups through policies instead of assigning access directly to each user.

---

## Example

A DevOps group may include users who need access to manage compute instances.

```text
Group: DevOps

Users:
- User 1
- User 2
- User 3
```

A policy can then be written for the DevOps group.

```text
Allow group DevOps to manage instance-family in compartment Development
```

---

## Why Groups Are Useful

Groups make access easier to manage.
Instead of writing separate permissions for every user, access can be managed at the group level. When a new user joins the team, the user can be added to the right group and receive the required permissions.

---

## What I Understood

My main understanding is that groups help keep access control clean.
Users should be placed into the correct groups, and policies should be written for those groups based on the required access.
