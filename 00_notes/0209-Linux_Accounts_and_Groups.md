# Types of Users

- Root User == Super User
    - NEVER run a service as a root user
- User Accounts (Standard users like v.weber)
    - sudo lets a standard user execute commands as super user
- Service Accounts (e.g. nginx)
    - Best Practice to run services

# User Management
- Windows allows users to centrally manage User Accounts & permissions
    - Active Directory (AD) or Entra-ID (formerly Azure AD)
    - This allows accessing your user account from any machine connected to the
      central user directory
- Linux does not have this capability natively

## Permission Management
- Give permissions to users directly
- Manage Permissions through User Groups
    - User Groups are collections of users that grant them specific permissions
    - A User always has all permissions that a group has
    - Users can be added to multiple groups (e.g. sudoers, docker)

### Access Control Files
- `/etc/passwd` -> Stores user account information
    - each line represents a user
    - username:password:uid(unique_id):gid(primary_group_id):gecos:homedir:shell
    - gecos = human readable user info (e.g. Full Name, E-Mai) comma separated
        - "Full Name","Room Number","Work Phone","Home Phone","Other"
        - user info might vary across distributions
    - a primary group with the name of the user is created by default 
- `/etc/group` -> lists all user groups

## Manage Users
- `adduser [username]`, `addgroup [groupname]`
    - interactive, all info can be input after executing the command
    - should be used from cli
- `useradd`,  `groupadd`
    - non-interactive, all info must be passed as parameters
    - should be used from scripts
- `deluser [username]`, `delgroup [groupname]`, `userdel`, `groupdel`
    - same difference as the add commands above
- `usermod` -> Modify a user account
    - add user to an additional group `usermod -aG [groupname] [usermod]`
- `gpasswd -d [username] [groupname]` -> remove user from a group
- `whoami` -> print username of logged in user to stdout
- `groups` -> which groups am I a part of?