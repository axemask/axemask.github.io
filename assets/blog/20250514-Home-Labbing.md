# Home Labbing

Date: May 14th, 2025
Author: Robert Crawford
Tags: Labbing, Networking, Administration, Learning

# Introduction

As I come close to graduating my Network Administration course, I am feeling like I have to solidify the theoretical knowledge I have learned by implementing hands-on projects. I know imposter syndrome is a common phenomenon in this field and I'm experiencing it more than ever now that I'm about to enter the workforce.

Not only do I feel like I'm lacking on the practical side of things, but I haven't had a whole lot of hands-on practice using different equipment and tools. In school we basically just used outdated Cisco routers and switches and the standard Windows and Fedora clients and while that's great and all I think there's so much more to tinker around with.

That's why I want to work on little projects such as this one so I can solidify the theoretical knowledge and experience different systems that may be used in different production systems. I want to become a versatile and effecient IT guru that's capable of working on any system in any environment.

I think labbing is a great way to learn because I am limited in terms of budget and in effect equipment but that's what I love about this field. You can do whatever you want using whatever tools you have available - just perhaps to a lesser degree.

For example, I don't have access to switches or routers that are capable of VLAN configurations but I've done a little research on the model of SOHO router I'm using and there is open source firmware that is flashable which enables such functionality so that's something I can implement at some point.

Anyways, that's enough rambling so let's move on to the details of my current lab environment and some goals I have.

# High-Level Details

## LAN Configuration

I'm not going to go into too much detail regarding the specific configuration of my entire home network for security purposes but I am using an old Linksys router that's isolating my lab environment from the rest of my LAN using double NAT. This probably isn't the _best_ solution but it's simple and easy to set up.

The state of the linksys router that I inhereted was using some shitty custom linksys firmware that had a bunch of cloud crap that I don't care about so I downgraded to the original Cisco firmware. I'm not sure what version of ASP.NET it was coded in but it feels like I'm working in Cisco packet tracer or something. Pretty neat 😎

## Server Configuration

I am only going to be using a single proxmox host as my type 1 hypervisor and everything will be virtualized using containers and VM's. That means all servers, routers, firewalls, etc. are going to be virtual.

The router I'm using has the capability of static routes so I might end up routing all WAN traffic through a virtualized firewall OS like pfsense later on but I'm already behind double NAT so I don't feel it super necessary at the current moment.

## Networking Configuration

Currently I'm only going to be using a single physical interface (vmbr0) to connect specific things to my LAN environment. I will create another bridge for internal network traffic (traffic between VMs on the proxmox host).

Later on, I may install and configure another physical interface for the firewall configuration I mentioned in the Server Configuration section above.

# TODO

Below is a list of goals that I plan on accomplishing. They are in no specific order:

- Install a DNS sinkhole such as pi-hole for ad free and tracker free browsing.
- Deploy a virtual firewall such as pfsense / opnsense and route all traffic through it.
- Flash a custom firmware such as DD-WRT, OpenWrt or FreshTomato on my SOHO router that allows VLAN configuration.
- (Long term) Potentially move hosting from GitHub pages to a container on my proxmox server???
- Deploy a media server for free TV / Movies in a totally legit and legal way that complies with all laws and regulations. 🏴‍☠️
- (Long term) Deploy a cloud solution
    - Research 