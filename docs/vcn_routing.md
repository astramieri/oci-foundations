# VCN Routing

VCN uses **Route Tables** to send traffic out of the VCN to the internet, to on-premises networks, or to peered VCN, and we look at each of these scenarios.

Route tables consist of a set of route rules. Each rule specifies a destination CIDR block and a route target (the next hop for the traffic that matches that destination CIDR block).

One thing to keep in mind is traffic within the VCN subnet is automatically handled by the VCN local routing. There's no entry in a route table needed for routing that data between the public subnet and the private subnet.

## Peering

If you have multiple networks, how do they talk to each other? 

1. Local Peering (same region)
2. Remote Peering (different regions)

![VCN Peering](../images/vcn_peering.png)

## Dynamic Routing Gateway v2

What happens if you have hundreds of VCNs?

![Dynamic Router Gateway v2](../images/drg_v2.png)