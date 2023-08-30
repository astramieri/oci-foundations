# Oracle Cloud Infrastructure Architecture

Core constructs of OCI's Physical Architecture:
- Regions: localized geographic area comprising of one or more availability domains. 
- Availability Domains (AD): fault-tolerant data centers located within a region but connected to each other by a low latency, high bandwidth network.
- Fault Domains (FD): grouping of hardware and infrastructure within an availability domain to provide antiaffinity.