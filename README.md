**Project: Hosting a Static Website on AWS**

**Overview:**
This project involves deploying a static HTML web application on AWS infrastructure. The deployment is orchestrated using various AWS services to ensure reliability, security, scalability, and fault tolerance.

**Deployment Steps:**
1. **Setup Virtual Private Cloud (VPC):**
   - Configured a VPC with public and private subnets across two availability zones to enhance fault tolerance and reliability.
   - Deployed an Internet Gateway to enable connectivity between VPC instances and the wider Internet.

2. **Established Security Groups:**
   - Implemented Security Groups as a network firewall mechanism to control traffic to instances.

3. **Utilized Multiple Availability Zones:**
   - Leveraged two Availability Zones to enhance system reliability and fault tolerance.

4. **Utilized Public Subnets:**
   - Utilized public subnets for infrastructure components like the NAT Gateway and Application Load Balancer.

5. **Secure Connections:**
   - Implemented EC2 Instance Connect Endpoint for secure connections to assets within both public and private subnets.

6. **Positioned Web Servers in Private Subnets:**
   - Placed web servers (EC2 instances) within private subnets for enhanced security.

7. **Internet Access for Private Subnets:**
   - Enabled instances in private application and data subnets to access the Internet via the NAT Gateway.

8. **Hosting the Website on EC2 Instances:**
   - Hosted the static website on EC2 instances within the private subnets.

9. **Load Balancing and Auto Scaling:**
   - Employed an Application Load Balancer and a target group for evenly distributing web traffic to an Auto Scaling Group of EC2 instances across multiple Availability Zones.

10. **Auto Scaling Group:**
    - Utilized an Auto Scaling Group to automatically manage EC2 instances, ensuring website availability, scalability, fault tolerance, and elasticity.

11. **Version Control and Collaboration:**
    - Stored web files on GitHub for version control and collaboration.

12. **Secured Application Communications:**
    - Secured application communications using a Certificate Manager.

13. **Monitoring and Alerting:**
    - Configured Simple Notification Service (SNS) to alert about activities within the Auto Scaling Group.

14. **Domain Registration and DNS Setup:**
    - Registered the domain name and set up a DNS record using Route 53 for routing traffic to the hosted website.

**Repository:**
The reference diagram and deployment scripts for this project are available in the GitHub repository. Please refer to the repository for detailed instructions on deploying the static website on AWS infrastructure.

**Conclusion:**
By following the instructions and utilizing the provided resources, you can successfully deploy a static HTML web application on AWS, ensuring high availability, security, and scalability.
