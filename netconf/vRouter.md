This file captures the  RESTCONF URI details for various NETCONF resources of Brocade 5600 vRouter.

| MX Command                                   | vRouter Model     | URI                                                                                                                                                                                                                   | Operation |
|----------------------------------------------|-------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------|
| configuration interfaces *input*             | vyatta-interfaces | http://{IP}:8181/restconf/config/network-topology:network-topology/topology/topology-netconf/node/vRouter/yang-ext:mount/vyatta-interfaces:interfaces/                                                                | GET       |
| set interfaces <input> *policy*              | vyatta-interfaces | http://{IP}:8181/restconf/config/network-topology:network-topology/topology/topology-netconf/node/vRouter/yang-ext:mount/vyatta-interfaces:interfaces/vyatta-interfaces-<type>:<type>/{tagnode}/bridge-group/         | PUT       |
| set system services dhcp-local-server dhcpv6 | vyatta-services   | http://{IP}:8181/restconf/config/network-topology:network-topology/topology/topology-netconf/node/vRouter/yang-ext:mount/vyatta-services:service/vyatta-service-dhcpv6-relay:dhcpv6-relay/listen-interface/{tagnode}/ | PUT       |
| set services service-set *input*             | vyatta-policy     | http://{IP}:8181/restconf/config/network-topology:network-topology/topology/topology-netconf/node/vRouter/yang-ext:mount/vyatta-policy:policy/vyatta-policy-route:route/                                                  | PUT       |