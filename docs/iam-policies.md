# IAM Policies

IAM policies define what access is allowed in Oracle Cloud Infrastructure.

A policy connects a subject, an action, a resource type, and a location.

---

## Basic Policy Format

Allow group <group-name> to <verb> <resource-type> in compartment <compartment-name>

---

## Policy Components

A policy usually includes:

- Subject: the group or dynamic group receiving access
- Verb: the level of access
- Resource type: the OCI resource being accessed
- Scope: the tenancy or compartment where the access applies

---

## Common Verbs

OCI policies commonly use these verbs:

inspect
read
use
manage

The access level increases from inspect to manage.

---

## Example Policies

Allow group DevOps to manage instance-family in compartment Development
Allow group NetworkAdmins to manage virtual-network-family in compartment Network
Allow dynamic-group app-instances to read buckets in compartment Storage


---

## What I Understood

My main understanding is that IAM policies must be written carefully.
A broad policy can give more access than required. A better approach is to define access based on role, resource type, and compartment scope.
