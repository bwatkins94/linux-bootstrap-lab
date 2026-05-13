# linux-bootstrap-lab

## Overview

This project uses Ansible to bootstrap and harden a fresh Ubuntu server in a repeatable, idempotent way.

It simulates a real-world infrastructure automaton workflow for provisioning Linux hosts with baseline packages, Docker, firewall rules, and SSH security hardening.

## Goals

- Practice production-style Ansible project structure
- Use resuable roles instead of one large playbook
- Demonstrate idempotent infrastructure automation
- Apply basic Linux server hardeninng
- Validate playbooks with CI checks

## Tech Stack
- Ansible
- Ubuntu Linux
- Multipass or local VM
- Docker
- UFW
- Fail2ban
- Github Actions

## Architecture

Local machine -> Ansible controller -> Ubuntu VM target

## Roles

### common

Installs baseline packages and configures the server environment.

### docker

Installs Docker, configures daemon settings, and enables the Docker service.

### security

Applies basic server hardening using UFW, SSH configuration, and Fail2ban

## Usage

Clone the repo:

'''bash
git clone https://github.com/YOUR_USERNAME/linux-bootstrap-lab.git
cd linux-bootstrap-lab