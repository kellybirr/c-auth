# C-Auth
This is my proposed "C-Auth" API Authentication Framework

C-Auth is heavily based on the core principals of *OAuth v2* for the authentication and authorization of API call between services and micro-services in homogeneous or heterogeneous systems.
  
The fundamental difference is that C-Auth issues and validates client and server TLS certificates instead of "tokens".  The certificates that are issued are used for both the authentication/authorization of API calls as well as the facilitation of TLS handshake and encryption so you can easily encrypt the traffic end-to-end within your service mesh.

At this time, C-Auth does not attempt to be a user identity framework.  A C-Auth equivalent of *Open-ID Connect* is out of scope today.

This repository will contain both the a server implementation in C# (.Net Core 2.2) as well as client implementations (initially only C#) and sample code.  I'll eventually also have "ready to deploy" Docker containers for this project. 

**CREDITS**
Significant portions of the core certificate issuing code in this project are based on the [AzureIoTDPSCertificates](https://github.com/rwatjen/AzureIoTDPSCertificates) project by [Rasmus W](https://github.com/rwatjen). 
