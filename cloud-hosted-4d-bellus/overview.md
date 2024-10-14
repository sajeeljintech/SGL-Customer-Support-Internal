# Overview

## Introduction

The ProxMox "Cloud" environment exists as a way for SGL to provide a hosted environment for our customers for our legacy 4D system.  This is decidedly a stop-gap solution that we hope to retire no later than the end of 2024.

## Why Have This

This enviroment is largely meant to support our smaller customers.  The advantages of the system are&#x20;

1. Rapid Deployment - Unlike how we have deployed onsite in the past we are able to deploy a new 4D Server (Customer Database) quickly in a reliable environment.
2. Server Purchase by Customer is NOT required - For smaller customers this saves on cost of purchasing a server and the time and effort for our techs to setup and configure the server.
3. Server Maintenance - Rather than relying on a customer to reliably maintain their server we are able to do this on a regular schedle.  It keeps their data more secure and safe
4. Easier Migration To Full Cloud - When we migrate users to the cloud it will be easier to migrate from this controlled environment rather than from a laptop server that may or may not be online reliably.

## VPN Connection

To access the environment the customer MUST first establish a VPN connection to our network.  There are many reasons for this but they include

1. Our cyber insurance requires we do not have open access to a Remote Desktop Server for Security reasons.
2. It maintains security for our data as well as our customers data.

### What is a VPN

Imagine you have a secret tunnel that connects your computer to another computer far away. When you use a VPN (Virtual Private Network), your internet traffic goes through this secret tunnel instead of traveling openly over the regular internet. This makes it harder for others to see what you're doing online.

It's like putting your internet connection inside a hidden, secure tunnel so that nobody outside can easily spy on your activities or see which websites you're visiting. VPNs help you stay safe and private while browsing the web.

### How Does a VPN Work?

When you connect to a VPN, your device first creates a secure connection to a VPN server. Think of it like a private, encrypted bridge connecting you to the server. This secure connection ensures that any data you send and receive while online is encrypted, meaning it is turned into a secret code that is difficult for others to read.

Once connected, the VPN server acts as a middleman between you and the internet. Instead of your internet traffic going directly from your device to the websites you visit, it first travels through the VPN server. This masks your original IP address and makes it look like your internet activity is coming from the VPN server, adding an extra layer of privacy.

So, the VPN works by encrypting your data and rerouting your internet traffic through a secure server, keeping your online activities private and secure.

## Remote Desktop

Our customers access their server by accessing a Remote Desktop environment that allows them access to the ShowGrounds Client software.  This client is setup to automatically connect to the correct 4D Server for that client. A user with access to more than one server will have a shortcut to more than one client application each pointing to a different server.

### What is Remote Desktop?

A Remote Desktop connection allows users to access and control a computer or server from a remote location over a network. This is typically done using Remote Desktop Protocol (RDP) software, which creates a virtual session that displays the remote device's desktop on the user's local screen. The user can interact with this session as if they were physically present at the remote machine, enabling them to use software, transfer files, and perform tasks just like they would on their local device. This is particularly useful for accessing resources and applications that are not available locally.

## ProxMox Server

### Virtualized Server Environment

A virtualized server environment allows multiple virtual servers to run on a single physical server. This is achieved through the use of hypervisor software, which creates and manages these virtual machines (VMs). Each VM operates independently, with its own operating system and applications, sharing the physical server's resources, such as CPU, memory, and storage. This promotes efficient resource utilization, reduces hardware costs, and simplifies management and scalability.

#### How It Works

1. **Hypervisor Layer:** The hypervisor, or virtualization manager, sits between the hardware and the VMs, allocating resources to each VM as needed.
2. **Resource Management:** Physical resources like CPU, RAM, and storage are virtualized and distributed among multiple VMs.
3. **Isolation:** Each VM is isolated, ensuring that the performance and security of one VM do not affect others.
4. **Flexibility:** VMs can be easily created, modified, and deleted based on usage requirements, making the setup highly flexible and scalable.

#### Specifics about ProxMox

ProxMox is an open-source virtualization management platform that integrates both Kernel-based Virtual Machine (KVM) and container-based virtualization (LXC) under one interface. It provides a robust, enterprise-class solution for running and managing virtual machines and containers. Key features include:

* **Web-Based Interface:** Centralized management through a user-friendly web interface.
* **High Availability (HA):** Supports clustering and HA configurations to ensure minimal downtime.
* **Backup and Restore:** Integrated backup solutions with snapshot functionality.
* **Resource Management:** Advanced resource allocation and monitoring tools.
* **Support for Multiple Storage Formats:** Allows use of various storage backends like local storage, NFS, iSCSI, and Ceph.
