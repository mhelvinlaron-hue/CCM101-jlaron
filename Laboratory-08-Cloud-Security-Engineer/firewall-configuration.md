# Firewall Configuration

## Allow SSH

```bash
sudo ufw allow ssh
```

This command allows SSH connections so I can manage the server remotely.

## Default Deny Policy

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

The first command blocks incoming connections unless they are allowed by a rule. The second command allows the server to send outgoing traffic.

## Allow Port 8080

```bash
sudo ufw allow 8080/tcp
```

This command permits TCP connections through port 8080 so users can reach the Nginx web application.

## What happens if you run sudo ufw enable before sudo ufw allow ssh?

The firewall may block my remote SSH connection if no rule allows it, which could prevent me from managing the server remotely.
