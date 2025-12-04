# “Design an AWS architecture for a highly scalable web application capable of handling 10,000 concurrent users.”

The architecture is designed for high scalability and availability to support 10,000 concurrent users.
Incoming traffic is routed through Route 53 to an Application Load Balancer in pubic subnets, which
distributes requests across EC2 instances in an Auto Scaling Group deployed in private subnets. Application
state is cached using ElastiCache (Redis) to reduce database load. The Database layer uses RDS/Aurora in
Multi-AZ deployment with optional read replicas for high availability

<img width="330" height="665" alt="Screenshot 2025-12-04 213415" src="https://github.com/user-attachments/assets/491a3a4d-367e-4ce8-9724-b7c288d91918" />
[AWS Architecture Diagram (draw.io)Task.pdf](https://github.com/user-attachments/files/23939593/AWS.Architecture.Diagram.draw.io.Task.pdf)
