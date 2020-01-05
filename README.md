# consul

Cluster

Servers (3,5) and Nodes

on Nodes places Services
на каждой ноде (узле) запущен agent 
общение с агентом происходит через localhost

DNS interface

nodes [node].node[.datacenter].[domain]

services [tag].[service-name].service.[datacenter].[domain]

by default domain = consul
default datacenter = dc1 and it can be omitted when requested for current dc 

examples:
```
dig @127.0.0.1 -p 8600 rls.service.consul.
dig @127.0.0.1 -p 8600 rls.service.consul. SRV
```
