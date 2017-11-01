# aws-template
templates and scripts for creating AWS components.

What's needed.
 - download and install the awscli
 - '.aws' folder in the $HOME folder of the user which will run the commands. 'mkdir ${HOME}/.aws'
 - create a new file called 'credentials'.  For each user create an entry like:
 
[default]
aws_access_key_id=<put your access key here>
aws_secret_access_key=<put your secret here>.


  you can create multiple entries in the file for each user and then when running the aws command you can stipulate which usr to reference. As you would expect 'default' is the 'goto' profile.
  
[default]
aws_access_key_id=<put your access key here>
aws_secret_access_key=<put your secret here>.
  
[isabelle]
aws_access_key_id=<put your access key here>
aws_secret_access_key=<put your secret here>.
  
 
 - create a new file called 'config' in the './aws' folder. example below.  the region simply tells the command which region I'm playing in.  and the output, tells './aws' how to present the output from the commands.  The options are, table, json or text.

[default]
region=eu-west-1
output=json
