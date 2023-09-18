# Compute Introduction

OCI Compute service provides you:
- virtual machines
- bare metal servers (full server completely dedicated to you)
- dedicated host (a bare metal machine where you can run VMs)

The three defining characteristics of this service include:
- scalability
- high performance
- lower pricing

## Flexible Shapes

Flexible Shapes means you have flexibility in choosing your own configuration. 

You could choose:
- Oracle Cloud Processor Units (OCPUs)
- Memory

NOTE. The number of virtual NICs and physical NICs are not customizable parameters for flexible shape compute instances.

In the cloud, there's this notion of **T-shirt sizing**. So you have a small, medium, large kind of shapes, and your application has to fit those shapes. And sometimes you over provision or under provision, and you have to go through that painful process of changing your machine types. With flexible shapes, you don't have to do that.

## What's the difference between dedicated host and VMs?

VMs are shared and multi tenant, meaning the host can be running VMs from multiple customers. But some customers want a dedicated host where they could run their own VMs and they don't have VMs from any other customer running there. 

## Choice of Processors

OCI is only one of the two cloud providers to provide you options on processors:
- AMD 
- Intel 
- Ampere (ARM-based processor)

## Preemptable VMs 

Preemptable VMs are low cost short lived VMs suited for batch jobs and fault tolerant workloads. These are similar to regular instances, but price 50% lower. So you can use them to reduce your cost further.
