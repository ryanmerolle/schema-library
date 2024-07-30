# Schema Library

## Main changes

- Split "Infra" namespace with proper DCIM / IPAM
- Move VRF to extension part

## Open topics

-[ ] Should we split DCIM to device and Device for instance? (as per nautobot)
-[ ] How can I add VLANs to IPAM section?
-[ ] For location the fact that the tree between simple and extended forces us to create 2 different extensions
-[ ] We can't add a "parent" statement in "extensions" section
-[ ] Putting enum (status, roles ...) in generics prevents users from editing ...
