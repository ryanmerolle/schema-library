# Schema Library

## Quick start

1. Create a branch

    ```console
    infrahubctl branch create testing-schema-library
    ```

2. Load base schema

    ```console
    infrahubctl schema load --branch testing-schema-library base/
    ```

3. Then pick and load extensions that fit your use case

    ```console
    infrahubctl schema load --branch testing-schema-library extensions/location_minimal
    infrahubctl schema load --branch testing-schema-library extensions/vrf
    infrahubctl schema load --branch testing-schema-library extensions/bgp
    ```

## Main changes

- Split "Infra" namespace with proper DCIM / IPAM
- Move VRF to extension part

## Open topics

- [ ] Should we split DCIM to Circuit and Device for instance? (as per nautobot)
- [ ] How can I add VLANs to IPAM section?
- [ ] For location the fact we have three (parent/child) forces us to create 2 different extensions
- [ ] We can't add a "parent" statement in "extensions" section
- [ ] Putting enum (status, roles ...) in generics prevents users from editing ...

## Progress

Base

- [x] Circuit
- [x] Dcim
- [x] Ipam
- [x] Location
- [x] Organization

Extensions

- [x] bgp
- [x] lag
- [x] location_extended
- [x] location_minimal
- [ ] qinq
- [x] tenancy
- [x] vrf

Experimental

- [ ] peering
- [ ] topology
- [ ] security

Next

- [ ] dns
- [ ] dhcp
- [ ] ntp
