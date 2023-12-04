# CloudFormation
Collection of AWS CloudFormation templates to serve as practice and reference for various designs

### Project 1
Very simplistic

### Project 2

### Project 3:
Started to learn that as I add more resources to templates I would need to change my naming conventions. The "projectWhatever" prefix was firstly redundant, and secondly unnecessary clutter. This one invovles a private subnet holding an EC2 instance and a public subnet with a NAT gateway. The goal was to practice creating a set-up that would allow outbound traffic from the private EC2 instance. I had to add EC2InstanceConnect to test this as that endpoint is necessary to have an instance connection to a EC2 instance that doesn't have a private IP address.
