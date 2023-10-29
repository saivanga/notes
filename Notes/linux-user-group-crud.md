# User & Group CRUD

1.  Create a new user:
    `sudo useradd -m -s /bin/bash <username>`
    This will create a new user account with the home directory /home/<username>.

1.  Add a user to a group:
    `sudo usermod -aG <group name> <username>`
    This will add the user to the group.

1.  Delete a user:
    `sudo userdel <username>`
    This will delete the user account.

1.  Change a user's password:
    `passwd <username>`
    This will allow you to change the password for the user.

1.  Lock a user account:
    `sudo passwd -l <username>`
    This will lock the user account, preventing the user from logging in.

1.  Unlock a user account:
    `sudo passwd -u <username>`
    This will unlock the user account, allowing the user to log in again.

1.  Grant sudo privileges to a user:
    `sudo usermod -aG sudo <username>`
    This will add the user to the sudo group, allowing the user to run commands with root privileges.

1.  Revoke sudo privileges from a user:
    `sudo usermod -G <username>`
    This will remove the user from the sudo group, preventing the user from running commands with root privileges.

1.  List all users on the system:
    `cat /etc/passwd`
    This will list all of the user accounts on the system, along with their home directories and shells.

1.  Get information about a specific user:
    `getent passwd <username>`
    This will provide information about the user, including their home directory, shell, and user ID.

1.  Change a user's home directory:
    `sudo usermod -d /new/home/directory <username>`
    This will change the user account's home directory to /new/home/directory.

1.  Change a user's shell:
    `sudo usermod -s /bin/zsh <username>`
    This will change the user account's shell to /bin/zsh.

1.  Set a user's expiration date:
    `sudo usermod -e 2023-10-31 <username>`
    This will set the user account's expiration date to 2023-10-31.

1.  Force a user to change their password at their next login:
    `sudo chage -d 0 <username>`
    This will force the user to change their password at their next login.

1.  Create a new group:
    `sudo groupadd <group name>`
    This will create a new group with the name that you chose.

1.  Delete a group:
    `sudo groupdel <group name>`
    This will delete the group.

1.  Add a user to a group:
    `sudo usermod -aG <group name> <username>`
    This will add the user to the group.

1.  Remove a user from a group:
    `sudo gpasswd -d <username> <group name>`
    This will remove the user from the group.

1.  List all groups on the system:
    `cat /etc/group`
    This will list all of the groups on the system, along with their members.

1.  Get information about a specific group:
    `getent group`
    This will provide information about the group, including its members.
