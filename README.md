# A-tech-networking_project

*  A bash script to connect to a private virtual machine.

To get started:
-  Turn the bastion_connect.sh into an executable by running:
   chmod u+x bastion_connect.sh


# Usage:
   Connect to the bastion/public instance.
-  ./bastion_connect.sh <PUBLIC_INSTANCE_IP>
   Connect to private instance/vm.
-  ./bastion_connect.sh <PUBLIC_INSTANCE_IP> <PRIVATE_INSTANCE_IP>
   Execute command on private instance.
-  ./bastion_connect.sh <PUBLIC_INSTANCE_IP> <PRIVATE_INSTANCE_IP> '<YOUR_COMMAND_GOES_HERE>'

# Performing Key Rotaion:
By doing this, you will successfuly perform an ssh-key rotation without breaking the bastion_connect.sh
Connect to the bastion/public instance.
1)  ./bastion_connect.sh <PUBLIC_INSTANCE_IP>
2)  bash ssh_keys_rotation.sh <PRIVATE_INSTANCE_IP>
3) continue using the bastion_connect.sh like before.
