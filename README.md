# Automation Platform Configuration

This repository contains the Automation Office platform configuration and inventory.

## Purpose

This repository serves as:

- Source of Truth for platform configuration
- AWX inventory repository
- AWX backup repository
- AWX to AAP migration repository
- Configuration as Code repository

It contains Ansible playbooks and roles to:

- Inventory existing AWX environments
- Export AWX configuration
- Assess migration readiness
- Generate platform reports
- Import configurations into AAP
- Validate migrations
- Document platform architectures

The framework uses:

- awx.awx
- configify.aapconfig

## Areas Covered

- Organizations
- Teams
- Users
- Credentials
- Projects
- Inventories
- Job Templates
- Workflow Templates
- Execution Environments
- Integrations

## Platform

Current Platform:
- AWX
- Kubernetes
- AWX Operator 2.19.1

Target Platform:
- Red Hat Ansible Automation Platform (AAP)

## Related Documentation

See /docs

## Use Cases

### Platform Assessment

Generate inventories and migration readiness reports.

### Configuration Export

Export AWX objects as Configuration as Code.

### Migration Readiness

Identify migration blockers before moving to AAP.

### AWX to AAP Migration

Export, transform, import and validate AWX configurations.

### Platform Documentation

Generate architecture and inventory reports.


## Workflow

Inventory
↓
Assessment
↓
Export
↓
Transform
↓
Import
↓
Validation
↓
Report


## Collections

This project requires:

- awx.awx
- configify.aapconfig


## Installation

Install required collections:
- requirements.yml
```yaml 
---
collections:
- name: awx.awx
- name: configify.aapconfig
```
- requirements.txt
```
requests
pyyaml
jmespath
```

## About

This repository is maintained as part of the TechPiece initiative focused on cloud, automation, Ansible and platform engineering.
- YouTube: [TechPiece](https://www.youtube.com/@techpieceio)
- LinkedIn: [Daniel Benitez Aguila](https://www.linkedin.com/in/danielbenitezaguila/?locale=es)

