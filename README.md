# Coding challenge
This coding challenge is about creating a simple application that will list all repositories for a given username/orgname from Github. The application should be written in Java with Spring and should be deployed to AWS EC2 instance using Terraform.

- [ ] Write an application in Java & Spring that will:
  - [ ] Expose a REST endpoint:
    - [ ] `GET /repos/{username/orgname}` (username/orgname from Github)
    - [ ] Call Github REST API to list all repositories for the given username/orgname
      - [ ] Use the following URL: `https://api.github.com/users/{username}/repos`
    - [ ] Return a list of repositories with the following information:
      - [ ] Full name
      - [ ] Description
      - [ ] Number of stars
      - [ ] Number of forks
      - [ ] Visibility
      - [ ] Default branch name
    - [ ] Handle HTTP errors and return a proper response
- [ ] Add Terraform configuration:
  - [ ] With provider set to region `us-east-1`
  - [ ] With a single EC2 instance:
    - [ ] AMI: `ami-0c55b159cbfafe1f0`
    - [ ] Instance type: `t2.micro`
    - [ ] User data that will install Java 11 and run the application
  - [ ] With a security group that allows inbound traffic on port 80
  - [ ] Protect the instance with the security group
- [ ] Run the workflow that will build and run the application with a provided username/orgname