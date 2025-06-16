# How to Use This Repository

## Prerequisites

- Ansible Automation Platform (AAP) version 2.5 already installed.
- AAP credential configured (either with username/password or token).
- Access to create Projects and Job Templates within the platform.

## Getting Started

To begin using this repository with a fresh AAP 2.5 installation, follow these steps:

### 1. **Create a Credential**  
Set up an Ansible Automation Platform credential that will be used in your Job Template.

![Create Credential](pictures/create-credential.png)

### 2. **Create a Project**  
Create a new AAP Project that points to this repository.

![Create Project](pictures/create-project.png)

### 3. **Set Up an Inventory**  
Use a demo inventory or any inventory that includes `localhost` as the only host.

![Set Up Inventory](pictures/setup-inventory.png)

### 4. **Create a Job Template**  
Create a Job Template using the credential, project, and inventory created above.  
Make sure to include an extra variable pointing to the `configs` directory in this repository.

```yaml
aap_configs_dir: /runner/project/configs
```

![Create a Job Template](pictures/create-job-template.png)
