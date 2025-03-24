# Coding challenge

- [ ] Write an application in Java & Spring that will:
  - [ ] Expose a REST endpoint that ...
- [ ] Add Terraform configuration:
  - [ ] With provider set to region `us-east-1`
  - [ ] With a single EC2 instance:
    - [ ] AMI: `ami-0c55b159cbfafe1f0`
    - [ ] Instance type: `t2.micro`
    - [ ] User data that will install Java 11 and run the application
  - [ ] With a security group that allows inbound traffic on port 80
  - [ ] Protect the instance with the security group
- [ ] Run the workflow that will build and test the application
- [ ] Run the workflow that will execute Terraform plan