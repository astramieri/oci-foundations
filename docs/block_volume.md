# Block Volume

Block Volume service provides persistent and durable storage to compute instances. The data is stored independently of the instance lifecycle Durable means we make multiple copies. So even if we lose one copy, we have other copies of the data available in the data center. 

Block Volume Tiers:
1. **Lower Cost**: large sequential I/O workloads (streaming data warehousing)
2. **Balanced**: balanced choice for random I/O (boot disks)
3. **Higher Performance**: most I/O-demanding workloads
4. **Ultra High Performance**: highest I/O-demanding workloads (relational databases)

In case of block volume, there is something which is called block volume performance unit. And basically, this includes the concept of **Volume Performance Units (VPUs)**. You can purchase more VPUs to allocate more resources to a volume increasing your IOPS per gig and through output per gig.

## Auto-Tune Performance

Auto-Tune Performance helps you save on the costs. It changes the volume performance to lower cost when the volume is detached. When the volume is reattached, the volume performance is automatically adjusted to the previous setting.

## Encryption

Encryption is turned on by default (you cannot turn this off). OCI offers also *encryption in transit*, meaning when your virtual machine is talking to the block storage service, the traffic is encrypted in transit between the virtual machine and the block service.

## Read/Write Shareable

Block service offers **read/write shareable feature** where a single disk can be shared with multiple VMs and these VMs can read and write to the single block volume.

## Resizing Block Volumes

1. **off-line resizing**
2. **on-line resizing**: you can expand the volume size without detaching the volume from an instance, so it keeps your applications up and running. 

## (Asynchronous) Replication of Block Volumes

Block Volumes are being replicated from one region to another region. 

Scenarios:
- disaster recovery
- migration
- business expansion

##  Volume Groups

Block Volume service provides you with the capability to group together multiple volumes in what we call as a volume group. This simplifies the process to create time consistent backups of running applications that span multiple volumes across multiple instances.