#  Brief explanation of how you designed the VPC and subnets

I designed a VPC using a /16 CIDR block to allowe enough IP addresses for future scalability. I created two public and two private subnets, each with /24 CIDRs for clean segmentation. The public subnets are routed to an internet Gateway, allowing inbound/outbound access. The private subnets use a NAT Fateway placed in the public subnet enable secure outbound internet access. Finally, I used Terraform to automate the entire VPC setup, making deployment and deletion consistent and repeatable.



<img width="1920" height="996" alt="Screenshot (1)" src="https://github.com/user-attachments/assets/aae5c38a-9d4d-4ab5-90d4-f82067aef2bb" />
<img width="1903" height="995" alt="Screenshot (2)" src="https://github.com/user-attachments/assets/b2fdbc6e-b83a-4cab-940f-882ad827dd91" />
<img width="1920" height="1010" alt="Screenshot (3)" src="https://github.com/user-attachments/assets/ade800b7-fb72-4996-938c-7360dec9006c" />
<img width="1920" height="1032" alt="Screenshot (4)" src="https://github.com/user-attachments/assets/42b87681-e500-4043-a451-ff9b0ebbc711" />
<img width="1899" height="933" alt="Screenshot 2025-12-04 203038" src="https://github.com/user-attachments/assets/67e4d2b2-d5f5-423a-a11a-e5fd9a640b25" />
