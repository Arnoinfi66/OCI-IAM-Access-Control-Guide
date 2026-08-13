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
