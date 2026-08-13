# Dynamic Groups and Instance Principals

Dynamic groups and instance principals are used when OCI resources need to access other OCI services.
This is useful because it avoids storing API keys directly on compute instances.

---

## Dynamic Groups

A dynamic group includes OCI resources based on matching rules.
For example, compute instances in a specific compartment can be included in a dynamic group.

Example rule:
ALL {instance.compartment.id = '<compartment_ocid>'}
