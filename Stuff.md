# 💡 Lessons Learned - Ansible

- [x] Set up Ansible
- [x] Build a invetoryfile
- [x] Using a module
- [x] InstallStuff via Ansible (*apt-module*)
- [x] RunServices via ansible (*service-module*)
- [x] CreateUsers via Ansible (*user-module*)
- [x] CreateGroups via Ansible (*group-module*)

---

# 🐼 Bootcamp Exercises - Exercises

### Create&Use InventoryFile - Challenge #1
+ Create 4 Linux VMs. One will be the Ansible control node and the other 3 the managed nodes.
+ Check that the control node can access the managed nodes using SSH.
+ Install Ansible on the control machine.
+ Create an inventory file that contains the managed nodes and gather them in a group called servers.
+ Test Ansible SSH authentication using the ansible command and the ping module.
### Extend Ansible Command - Challenge #2
+ Add behavioral inventory parameters for the username, password, and SSH port.
+ Run the ansible command without -u user -k to check that it uses the parameters from the inventory file.
 Challenge #3
+ Using the Ansible shell module and a Linux command, display the IP address of the default gateway of each managed node.
### Grep&Cut Modifcation - Challenge #4
+ Change the solution so that it redirects to a file the IP address (and ONLY the IP) of the default gateway of each managed node.
### ls - Challenge #5
+ Using the Ansible shell module and a Linux command, display the CPU on each managed node.
### useradd & tail Challenge #6
+ Using the Ansible shell module, create on each managed node a new user called toor that belongs to the sudo group. Run the command that creates the user as root.
+ Display the last created user on each managed node.
### apt - Challenge #7
+ On Ansible control node, create a shell script that synchronizes (mirrors) the /etc directory to /root/etc-backup
+ Using Ansible and the script module, run the script on each managed node.
### name=nginx - Challenge #8
+ Using Ansible and the apt module, install the nginx web server on each managed node.
### apt & upgrade=full - Challenge #9
+ Using Ansible and the apt module, upgrade all packages to their latest versions on each managed node
### service - Challenge #10
+ Using Ansible and the service module, restart SSH on all managed nodes.
### enabled - Challenge #11
+ Using Ansible and the service module, set nginx to start on boot on all nodes.
### group - Challenge #12
+ Using Ansible and the group module, create a group called managers on all nodes.
### user -Challenge #13
+ Using Ansible and the user module, create a user called toor on all nodes.
+ Add the user to the sudo and managers groups.
