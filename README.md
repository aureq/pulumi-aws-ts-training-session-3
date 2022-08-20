# Pulumi training using TypeScript (3rd session)
Exercises to learn how to use Pulumi (3rd session)

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
3. Create a virtual machine and ensure you can SSH into it
4. Create stack outputs for:
   * the VM host name
   * the VM default user name
   * the SSH private key as secret

### Bonus/Challenges ###

X. Use a 3rd pary module to compute subnets CIDR
Y. Generate a SSH key pair (ed25519) and pass it to the VM, verify you can SSH the VM
Z. Ensure the project can easily be configured (ie, no hardcoded values where possible)
A. Resources are tagged so it's easy to create an AWS Budget for cost tracking purpose

### Answers ###
You will find all the answers [here](answer/).