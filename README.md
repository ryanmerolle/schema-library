# Schema Library

## Main changes

- Split "Infra" namespace with proper DCIM / IPAM
- Move VRF to extension part

## Open topics

-[ ] Should we split DCIM to Circuit and Device for instance? (as per nautobot)
-[ ] How can I add VLANs to IPAM section?
-[ ] For location the fact we have three (parent/child) forces us to create 2 different extensions
-[ ] We can't add a "parent" statement in "extensions" section
-[ ] Putting enum (status, roles ...) in generics prevents users from editing ...

## Progress

Base
-[x] Circuit
-[x] Dcim
-[x] Ipam
-[x] Location
-[ ] Organization

Extensions
-[ ] Bgp
-[ ] Lag
-[ ] location_extended
-[ ] location_minimal
-[ ] qinq
-[ ] tenancy
-[x] vrf

Experimental
-[ ] peering
-[ ] topology
