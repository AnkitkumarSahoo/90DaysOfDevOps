**What is a container and why do we need them?**
Ans:
A container is a lightweight, standalone package that includes everything needed to run a piece of software:
It ensures the application runs the same way everywhere.
The most popular container platform is Docker.

**Containers vs Virtual Machines — what's the real difference?**
Ans:
A VM virtualizes hardware.
Each VM:
Has its own full operating system
Includes its own kernel
Is completely isolated
Structure:
Physical Server
 └── Hypervisor
      ├── VM 1 (Guest OS + App + Libraries)

A container virtualizes the operating system.
Containers:
Share the host OS kernel
Don’t include a full OS
Are lightweight and fast
Structure:
Physical Server
 └── Host OS
      └── Container Engine (Docker)
           ├── Container 1 (App + Libraries)

**What is the Docker architecture? (daemon, client, images, containers, registry) ** 
Docker follows a client-server architecture. The Docker client communicates with a background process, the Docker Daemon, which does the
heavy lifting of building, running, and managing your containers. This communication happens over a REST API, typically via UNIX sockets
on Linux (e.g., /var/run/docker.sock) or a network interface for remote management.



           
