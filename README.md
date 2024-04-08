# A-tech-networking_project

A bash script to connect to a private virtual machine.

## Getting Started

To make `bastion_connect.sh` executable, run the following command:

```bash
chmod u+x bastion_connect.sh
```
# Usage
```bash
Connect to the bastion/public instance:
./bastion_connect.sh <PUBLIC_INSTANCE_IP>

Connect to a private instance/vm:
./bastion_connect.sh <PUBLIC_INSTANCE_IP> <PRIVATE_INSTANCE_IP>

Execute a command on a private instance:
./bastion_connect.sh <PUBLIC_INSTANCE_IP> <PRIVATE_INSTANCE_IP> '<YOUR_COMMAND_GOES_HERE>'
```
# Performing Key Rotation
```bash
Perform an SSH key rotation seamlessly without affecting bastion_connect.sh:

Connect to the bastion/public instance:
./bastion_connect.sh <PUBLIC_INSTANCE_IP>

Execute the SSH keys rotation script:
bash ssh_keys_rotation.sh <PRIVATE_INSTANCE_IP>

Continue using bastion_connect.sh as before.

Just replace `<PUBLIC_INSTANCE_IP>` and `<PRIVATE_INSTANCE_IP>` with the actual IP addresses and `<YOUR_COMMAND_GOES_HERE>` with the command you wish to execute on the private instance. Enjoy your project!
```
