
# Create_AMI_using_Ansible-and-Packer

- Here is to create an AMI to host a PHP application in AWS EC2 instance.
- Using Packer and Ansible
- Create an IAM user with programmable access and note the access and secret keys.

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/azizulmaqsud/Create_AMI_using_Ansible-and-Packer.git
   ```
2. [Install Packer](https://www.packer.io/docs/install)
3. [Install Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)

### Creating AMI

AMI is created using Packer.

1. Set the environment variables: AWS_ACCESS_KEY_ID, AWS_SECRET_ACCESS_KEY
2. Update the default values of base_ami (amazon Linux), subnet_id (with internet access), and security_group_id (allow port 22 from local IP) in the variables.pkr.hcl to match the ones in your AWS account.
3. cd into the packer folder in the cloned repository.
4. Run the following commands in order
    - packer init .
    - packer fmt .
    - packer validate .
    - packer build .

This will provision the AMI in the AWS account.

Now, you can use the AMI to launch an EC2 instance with the web application pre-configured and ready to use.
## Thank You!
## Stay Connected !!

https://www.youtube.com/channel/UCNwP7KEElaJ7cdDTLP-KbBg

https://www.linkedin.com/in/azizul-maqsud/

https://azizulmaqsud-1684501031000.hashnode.dev/

https://medium.com/@azizulmaqsud

https://twitter.com/Sohail2me

https://github.com/azizulmaqsud
