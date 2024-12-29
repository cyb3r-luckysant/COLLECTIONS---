# ⚠️ Deprecated Linux Command Usage
---

| **🚫 Deprecated Command**     | **✅ Up-to-Date Alternative**              | **📖 Description**                                            |
|-------------------------------|--------------------------------------------|--------------------------------------------------------------|
| `ifconfig -a`                | `ip addr show` (or `ip a`)                 | Show all interfaces' details                                 |
| `ifconfig eth0 up/down`      | `ip link set eth0 up/down`                 | Enable or disable `eth0`                                     |
| `ifconfig eth0 10.0.0.5/24`  | `ip addr add 10.0.0.5/24 dev eth0`         | Assign an IP address to `eth0`                               |
| `ifconfig eth0 mtu 9000`     | `ip link set eth0 mtu 9000`                | Set MTU of `eth0`                                            |
| `ifconfig eth0 promisc`      | `ip link set eth0 promisc on`              | Enable promiscuous mode                                      |
| `ifconfig eth0 -promisc`     | `ip link set eth0 promisc off`             | Disable promiscuous mode                                     |
| `ifconfig eth0:0 10.0.0.8/24`| `ip addr add 10.0.0.8/24 dev eth0 label eth0:0` | Add a new alias with an IP address to `eth0`                |
| `ifconfig eth0 hw ether 11:22:33:44:55:66` | `ip link set dev eth0 address 11:22:33:44:55:66` | Change MAC address of `eth0`                               |
| `netstat`                    | `ss`                                       | Show all open sockets                                        |
| `netstat -tulpn`             | `ss -tulpn`                                | Show all listening TCP/UDP connections with PID info         |
| `route`                      | `ip route show` (or `ip r`)                | Show routes                                                  |
| `route add -net 192.168.2.0/24 dev eth0` | `ip route add 192.168.2.0/24 dev eth0` | Add a new route                                             |
| `route add default gw 192.168.2.1` | `ip route add default via 192.168.2.1`   | Add a default gateway                                       |
| `arp -a`                     | `ip neigh`                                 | Show ARP table                                               |
| `arp -s 10.0.0.10 11:22:33:44:55:66` | `ip neigh add to 10.0.0.10 lladdr 11:22:33:44:55:66 dev eth0` | Add a static ARP entry                                      |
| `arp -d 10.0.0.10`           | `ip neigh del 10.0.0.10 dev eth0`          | Remove an ARP entry                                          |

---

### 💡 Summary
This table highlights the **deprecated Linux networking commands** and their modern **iproute2** replacements. Using the latest commands ensures better functionality and support for modern Linux systems.

