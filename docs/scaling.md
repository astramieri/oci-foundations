# Scaling

There are two kinds of scaling:
- vertical scaling
- horizontal scaling

## Vertical Scaling (scale up/down)

Vertical scaling means that you are scaling up or down instance shapes. 

New shape must have the **same hardware architecture**. 

When you scale up or scale down there is a **downtime required**.

Good practice: stop your instance before any kind vertical scaling.

![Vertical Scaling](../images/vertical_scaling.png)

## Horizontal Scaling (Autoscaling) (scale out/in)

Horizontal Scaling means that you add more VMs of the same shape, or you take a bit more of the same shape. This enables large-scale deployment of VMs.

Why is this so popular and powerful? The reason it is so powerful is, it gives you that scaling capability, but it also gives you that **high availability** And a thing which makes it really powerful is, you can match traffic demand by adding to removing VMs **automatically**. There is no extra cost for using Autoscaling.

There are three steps you have to follow to get Autoscaling:
1. create a **template** (config): OS image, matadata, shapes, cNICs, etc.
2. create an **instance pool**: a collection of instance in advance
3. create the **autoscaling rules**: minimum size, maximum size, etc.

![Autoscaling Rules](../images/autoscaling_rules.png)