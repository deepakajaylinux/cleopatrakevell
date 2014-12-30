The Phlagrant
Synopsis
Installation
Requirements
Code for installing virtual box
Installation via Cleopatra
Installing Phlagrant alone
Methodologies in usage
Help command
Brief Example
Available modules and its uses
Synopsis
While comparing with Cleopatra, the Phlagrant is a virtual machine management tool that provides the features for Virtual machine and development environment management. 
By using Devops it manages the virtual machine configuration, facilitates the different types of contributors even in a highly complex development environment.
It facilitates the automating, standardizing and managing the setup to virtual environment. Its functionalities includes Configuration Management, Test Automation Management, Automated Deployment, Build and Release Management, Development Environment Management and those functionalities are performed with the aid of php.
In Phlagrant the Configuration Management, Systems Automation and Infrastructure is depends and based on php. Editing a php script is really easy, as there is no compilation step to perform
The Phlagrant is object-oriented that enrich not only the data type but also the types of operations that can be applied to the data. Hence, while comparing object-oriented programming techniques over procedural programming techniques , the object-oriented programming enables the end users to create modules that do not need to be changed when a new type of object is added.
The Phlagrant is extensible, as if any extra module is required the user can frame and design the module as per their requirements and they can include.
Installation
Pre-requirements
If you wish to use the Phlagrant, ensure whether the Virual box is installed in your machine, along with the Virtual box guest additions functionality
Code for installing virtual box:
sudo cleopatra virtualbox install --yes --guess --with-guest-additions
Installation
There is two possible ways to install the Phlagrant tool to your machine:
Installation via Cleopatra
Installing Phlagrant alone

Installation via Cleopatra
if you have Cleopatra tool in your machine, then it's simple to install the phlagrant by using the code as given below
sudo cleopatra phlagrant install --yes --guess
here the word guess can be ignored while selecting your own directory during installation.
Installing Phlagrant alone
If you want to install the phlagrant tool to your machine without depending on the Cleopatra tool, it is easier by using the command,
sudo apt-get install php5 git
this command will install php5 and git on your machine. After that use the following command,
git clone http://github.com/PharaohTools/phlagrant && sudo php phlagrant/install-silent
the command on the above mentioned can be used if you don't want to select the location during the installation. If you wish to do so, use the following command:
git clone http://github.com/PharaohTools/phlagrant && sudo php phlagrant/install
Methodologies in usage:
Here, let us see how to use the commands under the tool and its usage.
if you simply type the following command,
phlagrant
As shown in the below screenshot, you will get the display of all the modules available under this tool.

Help command:
It's simple to use the help command,
phlagrant ModuleName help
This command helps you how the particular modules works, and also about what are the actions it can perform.
The below screenshot explains you how the help command is used to explain the module Box.

Brief Example:
let's see about a short example regarding the phlagrant here.
create a directory, or simply use a current web project as your new Pharaoh project mkdir /var/www/my-test-project && cd /var/www/my-test-project
install virtualbox to your machine if you don't have it already, it's simple by using the command as follows,
 sudo cleopatra virtualbox install --yes --guess --with-guest-additions
add a default Cleopatra Configuration Management Autopilot file using the following command
sudo cleopatra cleofy install-generic-autopilots --yes --guess --template-group=phlagrant
flirtify phlagrant flirt now --template-group=default-php
install, configure and start the virtual machine Phlagrant up now
Available modules and its uses:
Box - Box - Manage Base Boxes for Phlagrant
Destroy - Destroy - Stop a Phlagrant Box
EnvironmentConfig - Environment Configuration - Configure Environments for a project
Flirtify - Phlagrant Flirtify - Generate a Phalgrantfile based on a template
Halt - Halt - Stop a Phlagrant Box
Logging - Logging - Output errors to the logging
Resume - Resume - Stop a Phlagrant Box
SystemDetection - System Detection - Detect the Running Operating System
Templating - Templating
Up - Up - Create and Start a Phlagrant Box
