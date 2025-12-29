# Terraform
Day 01 – Introduction to Infrastructure as Code (IaC)

Introduction:

In modern cloud environments, creating and managing servers manually is time-consuming and can lead to mistakes.

To overcome this, we use Infrastructure as Code (IaC).

Infrastructure as Code means managing infrastructure using code instead of manual configuration.

---

## What is Infrastructure as Code (IaC)?

IaC is a method of creating and managing:

- Servers
- Networks
- Databases
- Storage

using configuration files.

These files can be stored in GitHub and reused whenever needed.

---

## Why IaC is Important

- Reduces manual errors
- Saves time
- Makes infrastructure repeatable
- Easy to track changes using Git
- Supports automation and DevOps practices

---

## Types of Infrastructure as Code Tools

There are **three main types of IaC tools**.

---

## 1. Configuration Management Tools

**Examples:** Ansible, Puppet, SaltStack

- Used when a server already exists
- Helps install and manage software on that server

### Example

If a server is already running and you want to install Apache, Nginx, or other packages, configuration management tools are used.

---

## 2. Server Templating Tools

**Examples:** Packer, Docker

- Used to create pre-configured server images
- OS and required software are already installed
- Helps reuse the same image multiple times

---

## 3. Provisioning Tools

**Examples:** Terraform, AWS CloudFormation

- Used to create cloud resources like:
    - Servers
    - Databases
    - Networks
    - Storage

Terraform supports multiple cloud providers, while AWS CloudFormation works only with AWS.