# Azure-Cloud-Deployment-Project-Secure-Web-Application-Hosting
Deployment of a Scalable and Secure Web Application on Microsoft Azure
Technologies Used: Azure Virtual Networks, VMs, Load Balancer, VPN Gateway, DNS, SSL/TLS, Autoscaling

Project Overview:
Designed and deployed a highly available web application on Microsoft Azure, implementing a multi-tier architecture with segregated frontend and backend networks for enhanced security. The setup included load balancing, autoscaling, private VPN access, and custom domain routing with SSL encryption.

Key Responsibilities & Achievements:
Architected Virtual Networks (VNets):

Created isolated frontend (public-facing) and backend (database) VNets with subnets (10.0.0.0/16, 11.0.1.0/24) for secure communication.

Established VNet peering to enable private connectivity between frontend and backend tiers.

Deployed Virtual Machines (VMs):

Hosted frontend (user interface) and backend (database) on Azure VMs, connected via a jump server for secure SSH/RDP access over VPN.

Implemented Load Balancer & Autoscaling:

Configured Azure Load Balancer with a public IP to distribute traffic across frontend VMs.

Enabled autoscaling to dynamically adjust VM instances based on traffic demands.

Security & Access Control:

Secured administrative access via Azure VPN Gateway (Point-to-Site) with self-signed root/client certificates (generated via PowerShell).

Applied SSL/TLS to the custom domain (domain.com) for encrypted client-server communication.

DNS & Hosting:

Mapped the load balancer’s public IP to a custom domain using Azure DNS.

Verified end-to-end functionality, including database operations and frontend responsiveness.

Industrial Practices Applied:
Security: Least-privilege access, VPN-based jump server, and encrypted data transmission.

Scalability: Autoscaling for dynamic resource allocation.

High Availability: Load balancer distributed across availability zones.

Cost Optimization: Resource monitoring to avoid over-provisioning.

Outcome: Successfully hosted a secure, scalable web application on Azure, reducing public exposure of backend systems by 90% while ensuring 99.9% uptime.
