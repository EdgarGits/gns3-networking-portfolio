# Laboratorio 02: Static routes

##  Description
Laboratory on **GNS3** to learn about **Static routes** on a router. A static route on a Cisco router is a manually configured path used to direct traffic to a specific destination network

##  Topology
* **Router (R1):** .
  * `S`: `10.1.0.0/24` via `10.1.0.2`
  * `S`: `10.1.1.0/24` via `10.1.0.2`
* **Router (R2):** .
  * `S`: `10.0.1.0/24` via `10.0.0.1`
  * `S`: `10.0.2.0/24` via `10.0.0.1`
  * `S`: `10.1.1.0/24` via `10.1.0.1`
* **Router (R3):** .
  * `S`: `10.0.0.0/24` via `10.1.0.2`
  * `S`: `10.0.1.0/24` via `10.1.0.2`
  * `S`: `10.0.2.0/24` via `10.1.0.2`


##  Key commands to check the configuration
Checking the routes:
```text
show ip route
