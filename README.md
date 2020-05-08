# Deploy-Infrastructure-as-Code-IAC-
Deploy a high-availability web app using CloudFormation

                                      Diagram of Udagram Project
![](Udacity%20Project-2%20Diagram.jpeg)

In this project, you’ll deploy web servers for a highly available web app using CloudFormation.
There will be two parts to this project:

You'll first develop a diagram that you can present as part of your portfolio and as a visual aid to understand the CloudFormation script.
The second part is to interpret the instructions as well as your own diagram and create a matching CloudFormation script.

It is a best practice to separate infrastructure networks and infrastructure servers script files and their corresponding script parameters files. The insfrastructures in the diagram above have been created one by one and been validated on the AWS console. This way it is easier to debug the errors you run into instead of creating the stacks all at once.

##Instructions to deploy:
######Run below code to create a network stack
./create.sh UdagramApp my_infrastructure_network.yml my_infrastructure_network_params.json

######After the stack is created run the below code to update it with additional infrastructures
.update.sh UdagramApp my_infrastructure_network.yml my_infrastructure_network_params.json

######Run below code to create a server stack
./create.sh UdagramApp my_infrastructure_servers.yml my_infrastructure_servers_params.json

######After the stack is created run the belwo code to update it with additional infrastructures
./update UdagramApp my_infrastructure_servers.yml my_infrastructure_servers_params.json

##Files incuded are:
create.sh - CloudFormation create stack script
update.sh - CloudFormation update stack script
destroy.sh - CloudFormation delete stack script
my_infrastructure_network.yml - Udagram Project's CloudFormation network script
my_infrastructure_network_params.json - Udagram Project's CloudFormation network parameters script
my_infrastructure_servers.yml - Udagram Project's CloudForamtion server script
my_infrastructure_servers_params.json - Udagram Project's CloudFormation server parameters script




