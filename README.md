# Build Ubuntu 20.04 Customized ami in AWS

## Requirements

  - [Packer](http://www.packer.io/)
  - AWS account access key and secret key
  - Ansible roles to customized ami 

## Usage

Clone repo, fill variables details in vars.json file. 

Add your own ansible roles under ansible/roles directory and define under roles in ansible/main.yml.  

Run build.sh

    $ ./build.sh 
    
Packer will create your customized ami and copy to your destination aws regions defined in vars.json. 