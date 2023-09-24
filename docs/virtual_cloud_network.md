# Virtual Cloud Network

A **Virtual Cloud Network** (VCN) is a private software defined network in Oracle Cloud. It's used for secure communication. It lives in an OCI region.

A VCN is a virtual, private network that you set up in Oracle data centers in a single OCI region. It resembles a traditional network, with firewall rules and specific types of communication gateways that you can choose to use. A VCN spans all the availability domains in the region.

## VCN Address Space

VCN has an **address space** (IP addressing range). You take that range and break it down into smaller networks which are called *subnetworks*. And these subnetworks are where you would instantiate your compute instances.

![VCN Address Space](../images/vcn_address_space.png)

## VCN Communications

What different mechanisms exist inside a VCN ?

1. **Internet Gateway**: two-way communication between a VCN and the internet.
2. **NAT Gateway**: one-way communication from a VCN to the internet.
3. **Service Gateway**: access from a VCN to public Oracle services.
4. **Dynamic Router Gateway (DRG)**: access from a VCN to destinations others than the internet (e.g. on-premises networks or another VCN in the same/different region.).

A Service Gateway in Oracle Cloud Infrastructure networking service enables access to Oracle services within the same region without the traffic going through the public internet. This provides a more secure and reliable connection for accessing Oracle services like Object Storage, Autonomous Database, and others.

![Communication Internet](../images/vcn_internet.png)

![Communication On-Premises](../images/vcn_on_premises.png)
