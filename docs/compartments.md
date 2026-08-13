# Compartments in OCI

Compartments are logical containers used to organize OCI resources.

They help separate resources by environment, team, application, or business function.

Compartments are also important because IAM policies can be scoped to a specific compartment.

---

## Example Compartment Structure

Root Tenancy
|
|-- Development
|   |-- Compute
|   |-- Storage
|
|-- Production
    |-- Application Servers
    |-- Databases

---

## Why Compartments Matter

Compartments help in three main areas:

- Organizing cloud resources
- Applying access boundaries
- Supporting ownership and control

For example, a user group may be allowed to manage resources only in the Development compartment, while access to Production remains restricted.

---

## Example Policy

Allow group DevOps to manage instance-family in compartment Development

This policy allows the DevOps group to manage compute-related resources only in the Development compartment.
---

## What I Understood

My main understanding is that compartments are not just folders.
They are part of the access control model in OCI. Policies use compartments to define where access applies.
