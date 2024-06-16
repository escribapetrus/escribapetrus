---
title: "Network"
author: "P. Schreiber"
date: "2024-05-30"
---

# API Gateway

An API gateway is a server that handles network requests from clients 
to backend services. Some of its responsibilities include:
- processing multiple concurrent requests (API calls);
- traffic management;
- authentication and authorization;
- monitoring;
- API version management;

API gateways manage and route networks and responses in modern architectures
such as microservices, providing a centralized point for routing, enforcing
security, monitoring, and transforming requests and responses.

The API gateway operates at the application layer of the OSI model, managing
HTTP/HTTPS API semantics.

## Features

Clients send requests to the API gateway instead of directly to backend services.
The API gateway routes the requests to the appropriate services.

Routing is done based on the request path, HTTP headers, or other
relevant criteria.

The API gateway can aggregate data from multiple sources into a single response,
when one request depends on multiple services.

The API gateway can enforce security policies, validating API keys and bearer
tokens used in OAuth authentication and authorization, blocking unauthorized
requests from reaching the backend services.

The API gateway can implement rate limiting and throttling policies to prevent
crashes due to excessive load and DDOS attacks.

The API gateway can implement caching strategies to deliver responses quickly,
reduce load on the backend services, and decrease latency.

The API gateway can log information about requests and responses, to provide
metrics and monitoring (observability).

The API gateway can transform requests and responses, by modifying headers and
content, or converting data formats such as JSON, XML and Protobuf.

## Justification

API gateways simplify the architecture, providing a single entry point instead
of tens or hundreds. They also decouple clients and services as they provide
a standardization of request and response formats.

API gateways also provide a unified system for concerns that different systems
may have, such as rate limiting and security.

API gateways may provide APIs in different protocols, enabling multiple forms
of communication with backend services.

## Examples
- **Kong:** open-source API gateway and microservices management layer;
- **NGINX:** reverse proxy, load balancer, HTTP cache, and API gateway;
- **AWS API Gateway:** AWS API management service;
- **Apigee:** Google Cloud API management service.

# Load Balancer

Load Balancers are applications that sit in front a distributed system 
application and distribute traffic across multiple servers to reduce
load on single servers, providing high availability and reliability.

They are used to ensure even distribution of traffic across server replicas.
Some features include: 
- traffic distribution using algorithms such as round-robin,
  least connections, hashing;
- health checks that monitor the servers' status; 
- failover by allowing routing only to healthy servers, and recovery by restart.

The difference to API gateways is that an API gateway routes traffic to 
different services in a distributed system, and load balancers route traffic
to different server replicas of a single service.

Load balancers operate at different layers of the OSI model:
- layer 7 for HTTP/HTTPS traffic;
- layer 4 for TCP/UDP traffic

# Reverse Proxy

Reverse Proxy is a handler for requests from clients to servers, providing 
anonimity, security, and performance enhancements. Some features include:
- anonimity, by masking the IP addresses of backend servers;
- security, protecting servers from direct exposure to the internet;
- load balancing, distributing requests across multiple servers;
- caching, storing responses to reduce load on the backend server.

Reverse proxies operate at the application layer (layer 7) of the OSI model,
dealing mostly with HTTP/HTTPS requests.

# OSI model

The OSI model is a set of standards for networks and network systems, ensuring
different technologies can communicate. It is divided in seven layers:

1. physical layer;
2. data link layer;
3. network layer;
4. transport layer;
5. session layer;
6. presentation layer;
7. application layer.

The OSI model is a foundational concept in networking. Each layer has specific
roles, and interacts with adjacent layers, ensuring data transmission from the
physical medium to the application level.

## Physical (layer 2)

The physical layer deals with the physical connection between devices,
sending and receiving raw bit streams over physical medium (cables, switches).

Physical layer protocols include:
- Ethernet;
- USB;
- Bluetooth.

## Data link (layer 2)

The data link layer provides node-to-node data transfer and error detection
and correction. It deals with data packets, handling MAC addresses,
checking errors (CRC), and controlling data flow.

Data link layer protocols include:
- Ethernet (MAC);
- PPP;
- HDLC;
- Wi-Fi (802.11)

## Network (layer 3)

The network layer manages data transfer between different networks. It deals
with logical addresses (IP), routing, and packet forwarding.

Network layer protocols include:
- IP (IPv4, IPv6);
- ICMP;
- ARP;
- RIP;
- OSPF.

## Transport (layer 4)

The transport layer ensures end-to-end communication and data transfer. 
It provides segmentation, flow control, error correction, reliable transmission,
and connectionless transmission (UDP). 

Transport layer protocols include:
- TCP;
- UDP;
- SCTP.

## Session (layer 5)

The session layer manages sessions or connections between applications. 
It establishes, maintains, and terminates sessions, session checkpoints,
and recovery.

Session layer protocols include:
- NetBIOS;
- RPC;
- PPTP.

## Presentation (layer 6)

The presentation layer translates data between the application layer 
and the network. It deals with data translation, encryption and decryption,
and compression.

Presentation layer protocols include:
- SSL/TLS;
- JPEG;
- MPEG;
- GIF.

## Application (layer 7)

The application layer provides network services directly to user applications.
It deals with interfaces for network services, such as email, file transfer,
web browsing.

Application layer protocols include:
- HTTP/HTTPS;
- FTP;
- SMTP;
- DNS;
- Telnet;
- SSH.

# Ingress vs Egress

Ingress and egress are terms that refer to the inbound and outbound flow
of data in a network system.

## Ingress

Ingress is the traffic and data packets that enter a network coming from
exteral sources. Managing ingress traffic is essential for controlling what 
enters the network and ensuring only legitimate and safe data is allowed.

Security measures include filtering and firewall rules to block unwanted 
or harmful traffic. Monitoring is employed to detect and prevent potential
threats such as DDOS attacks.

## Egress

Egress is the traffic and data packets that exit a network device, heading
to external destinations. Controlling egress traffic prevents data leaks
and ensure that internal systems do not communicate with malicious or
unauthorized external entities.

Security measures include filtering and firewall rules to prevent data leaks
and controle what data can leave the network. Monitoring is employed to detect
unusual or unauthorized data extrafiltration.










