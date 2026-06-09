# Evidence Collection

## Screenshot 01 — Security Group Restriction

File:

screenshots/01-security-group-restriction.png

Description:

AWS Security Group configured to allow SSH access only from an authorized public IP address.

Security Significance:

Reduces exposure to internet-wide SSH scanning and unauthorized connection attempts.

---

## Screenshot 02 — Successful SSH Connection

File:

screenshots/02-ssh-login-success.png

Description:

Successful SSH authentication into the Ubuntu Bastion Host using key-based authentication.

Security Significance:

Verifies secure remote administrative access.

---

## Screenshot 03 — System Update

File:

screenshots/03-system-update-complete.png

Description:

Execution of system package updates using apt.

Commands:

sudo apt update

sudo apt upgrade -y

Security Significance:

Reduces exposure to known vulnerabilities by applying available security patches.

---

## Screenshot 04 — UFW Firewall Enabled

File:

screenshots/04-ufw-firewall-active.png

Description:

Host-based firewall enabled with SSH access allowed.

Security Significance:

Provides an additional security layer beyond AWS Security Groups.

---

## Screenshot 05 — Authentication Log Review

File:

screenshots/05-authentication-log-review.png

Description:

Review of authentication and login activity on the Bastion Host.

Security Significance:

Provides visibility into administrative access and potential unauthorized login attempts.
