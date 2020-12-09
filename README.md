# dovecot-helper-scripts
Bash scripts for Dovecot administrator (virtual users, self-signed cert creation, and other)

###### genemailkeys - script for genering self-sigend cerificate to Dovecot

###### dcadduser - add user to Dovecot passwd-file

Use: `dcadduser <username> <password>` or run this script without parameters. If this script run without parametes, username and password will be requested in interactive mode.

Example: `dcadduser paulzovatel@example.org passw0rd666`

###### dcdeluser - delete user from Dovecot passwd-file

Use: `dcdeluser <username>`

Example: `dcadduser paulzovatel@example.org`

###### dcpasswd - change user password

Use: `dcpasswd <username> [new_password]` or `dcpasswd <username>`

Example: `dcpasswd paulzovatel@example.org nEw!pAssW0Rd` or `dcpasswd paulzovatel@example.org`

If run this script without `[new_password]` parameter, new password will be requested in interactive mode.

###### dclistuser - print list users from Dovecot passwd-file

##### v 0.2

Into scripts `dcadduser`, `dcdeluser` and `dcpasswd` added variable DOMAIN.

Set this variable for adding `@` and domain name after username (e.g. `DOMAIN="example.org"`)