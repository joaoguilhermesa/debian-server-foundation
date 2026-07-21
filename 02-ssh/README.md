# SSH (Secure Shell)

## Scenario

A computer administrator needs to verify that the SSH service is running properly and establish a remote connection to another computer.

## Objective

Learn how to install, configure, and use the SSH service for remote administration of Debian servers.

## Environment

- Operating System: Debian 13
- Window Manager: i3wm
- User: debian

## Install OpenSSH Server

```bash
sudo apt update
sudo apt install openssh-server -y
```

## Verify the SSH Service Status

```bash
sudo systemctl status ssh
```

This command checks whether the SSH service is running correctly.

![SSH Service Status](Images/01-ssh-status.png)

## Start the Service

```bash
sudo systemctl start ssh
```

## Enable the Service at Boot

```bash
sudo systemctl enable ssh
```

## Restart the Service

Restart the SSH service after making configuration changes.

```bash
sudo systemctl restart ssh
```

## Connect to Another Computer

```bash
ssh user@192.168.1.100
```

## SSH Configuration File

```text
/etc/ssh/sshd_config
```

## Restart SSH After Configuration Changes

```bash
sudo systemctl restart ssh
```

## Verify That Port 22 Is Listening

```bash
sudo ss -tlnp | grep ssh
```

![Port 22 Listening](Images/03-ss22.png)
## What i Learned

- Install the OpenSSH server
- Manage services with systemd
- Identify the main SSH configuration file
- Restart the SSH service after configuration changes
- Verify that the SSH service is listening on port 22
