# Pulumi training using TypeScript (3rd session)
Exercises to learn how to use Pulumi (3rd session)

## Introduction ##

In this session, you will learn how to create a ully functional VPC and a virtula machine. You'll also learn how to use 3rd party library to perform tasks more efficiently and in a reliable way. You'll have another opportunity to use string concatenation on Output<T>.

## Content ##

0. Create an `exercise` folder and switch to it
1. Create a new TypeScript project for AWS using AWS Classic
2. Create the following resources, and make sure they are all nested under the correct parent
   * A VPC (10.42.0.0/16)
   * An Internet Gateway
   * A public Subnet
   * A security group and allow port 22 inbound
   * A route table
   * Associate the route table and the subnet together
3. Create a virtual machine
   * using a free-tier instance type (reminder only - so your account doesn't get charged)
   * using the most recent Debian 11 AMI
   * ensure you can SSH into it
4. Create stack outputs for:
   * the VM host name
   * the VM default user name
   * the SSH private key as secret

### Bonus/Challenges ###

5. Use a 3rd pary module to compute subnets CIDR
6. Generate a SSH key pair (ed25519) and pass it to the VM using user-data, verify you can SSH the VM (as 'admin')
7. Ensure the project can easily be configured (ie, no hardcoded values where possible)
8. Resources are tagged so it's easy to create an AWS Budget for cost tracking purpose

### Answers ###
You will find all the answers [here](answer/).