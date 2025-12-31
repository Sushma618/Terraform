# Day 01 – Introduction to Infrastructure as Code (IaC) & Terraform

## Introduction
In modern cloud environments, creating and managing servers manually is time-consuming and can lead to mistakes.  
To overcome this, we use **Infrastructure as Code (IaC)**.

Infrastructure as Code means **managing infrastructure using code** instead of manual configuration.

---

## What is Infrastructure as Code (IaC)?
IaC is a way of creating and managing:
- Servers
- Networks
- Databases
- Storage

using **configuration files**.  
These files can be stored in **GitHub** and reused whenever needed.

---

## Why IaC is Important
- Reduces manual errors  
- Saves time  
- Makes infrastructure repeatable  
- Easy to track changes using Git  
- Supports automation and DevOps practices  

---

## What is Terraform?
Terraform is an **Infrastructure as Code and infrastructure automation tool**.

With Terraform, we can create and manage cloud resources such as:
- Servers (EC2)
- Storage (S3)
- Networks (VPC)

---

## Terraform Basics (Required)
- Created by **Mitchell Hashimoto** in **2014**
- Uses **declarative approach** (define what we want)
- Uses **HCL (HashiCorp Configuration Language)**
- Terraform tool is written in **Go language**
- Follows **DRY principle (Don’t Repeat Yourself)**

---

## Terraform Providers
- Providers tell Terraform **where to create infrastructure**
- Without a provider, Terraform does not know which cloud to use
- Every Terraform project starts with a **provider block**

---

## Terraform Resources
- Resources represent **real infrastructure objects**
- Examples:
  - EC2 instance
  - S3 bucket
  - VPC

Resources are defined using a **resource block**.

### Resource Structure
```hcl
resource "<TYPE>" "<NAME>" {
  arguments
}


Type → What resource to create (example: aws_instance)

Name → Logical name used inside Terraform

Arguments → Resource details (AMI, instance type, tags)






Types of Infrastructure as Code Tools
1. Configuration Management Tools

Examples: Ansible, Puppet, SaltStack

Used when a server already exists

Helps install and manage software on that server

2. Server Templating Tools

Examples: Packer, Docker

Used to create pre-configured server images

OS and required software are already installed

Helps reuse the same image multiple times

3. Provisioning Tools

Examples: Terraform, AWS CloudFormation

Used to create cloud resources such as:

Servers

Databases

Networks

Storage

Terraform supports multiple cloud providers, while AWS CloudFormation works only with AWS.
