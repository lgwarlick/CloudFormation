# CloudFormation
Collection of AWS CloudFormation templates (YAML) to serve as practice and reference for various designs

## Lessons/Preferences Learned

### YAML vs JSON
I went with YAML for all of these templates one, because I think it's easier to ready and two, I was getting plenty of JSON template practice on the Azure side of things with ARM templates

### Parameter References
I was initially confused at !Ref parameter versus Ref:, but I ultimately settled on using the latter though I don't have strong feelings one way or the other. Many of the early project templates will show !Ref before I settled on a consistent format

### Naming Conventions
I didn't find any hard and fast "best practice" for naming conventions as it related to CloudFormation templates. I went with camelCase because I had used it for the longest. Originally, as reflected in the early templates, I went for projectNumberResourceName (e.g. projectTwoIGW), but as the templates got more lengthy and complex that became messy. It also didn't make much sense considering the project number was already implied by the template name. I did, however, keep a version of this for parameters meaning that everything definied in that second of the template would be, for example, parameterEC2Instance. When it came to making edits I personally found this to make it easier to track down where in the template I needed to be.

### Project 1
Very simplistic

### Project 2

### Project 3:
Started to learn that as I add more resources to templates I would need to change my naming conventions. The "projectWhatever" prefix was firstly redundant, and secondly unnecessary clutter. This one invovles a private subnet holding an EC2 instance and a public subnet with a NAT gateway. The goal was to practice creating a set-up that would allow outbound traffic from the private EC2 instance. I had to add EC2InstanceConnect to test this as that endpoint is necessary to have an instance connection to a EC2 instance that doesn't have a private IP address.
