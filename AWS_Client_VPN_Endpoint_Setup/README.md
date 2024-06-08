# This is a step-by-step tutorial on AWS Client VPN Endpoint setup to achieve secure, scalable, and highly available remote VPC connectivity.

We all know local network communication is more secure than public network communication. AWS Client VPN is a method to access ec2 servers and other AWS resources remotely using its private network as if we are connecting it locally.

# Need for VPN

To access the resources security, big organisations primarily use site-site VPN or AWS direct connect services. It helps in setting up a hybrid cloud network with secure access to Cloud resources from the data center/office network.

These options are quite expensive and only organizations with good project budget can implement these solutions as it requires a physical VPN device.

The next option is to have a client to site VPN connectivity. You can implement this using solutions like OpenVPN on a ec2 instance. Custom implementation requires expertise in managing a secure and highly available VPN service.

Or use AWS managed AWS Client VPN Endpoint service where you dont have the administrative overhead of managing the VPN server on AWS. All the patching and VPN high availability are taken care by AWS.

# What is AWS Client VPN?

AWS Client VPN is a fully managed VPN service that helps remote users securely access AWS resources.

This service will create an encrypted SSL connection between the client (PC, and mobile devices) and the AWS servers. It means the data transferred between your devices and AWS services is secure and protected.

The endpoint is managed by AWS and the users establish the connection using a client VPN application (OpenVPN).

Following are the key features of AWS Client VPN.

- Remote Access: Provides an encrypted TLS connection between the client and the remote server. This ensures the secure communication between the servers.
- Multi-Platform VPN Clients: Client application supports various operating systems such as Windows, Mac OS, Linux, Android, etc.
- Authentication: Mutual authentication and User-based authentication enables enhanced access control security.
- Certificate Management: The Client VPN Endpoint can utilize certificates from the AWS Certificate Manager.
- Client Configuration: The client VPN endpoint provides a multi-platform supported client configuration file to connect to VPN endpoint.
Scalability and Availability: Supports automatic scaling based on the client connections.
- Tunneling Types: The client endpoint supports two types of tunneling methods such as split tunneling and full tunneling.
AWS Client VPN Workflow

