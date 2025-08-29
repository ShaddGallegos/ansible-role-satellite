# Ansible Role Satellite

**Created:** May 2024

## Synopsis

An Ansible role for managing Red Hat Satellite installations, configurations, and operations. Provides automated deployment, configuration management, and maintenance tasks for Red Hat Satellite infrastructure.

## Supported Operating Systems

- Red Hat Enterprise Linux 7/8/9
- CentOS 7/8 Stream
- Rocky Linux 8/9
- AlmaLinux 8/9

## Quick Usage

### Basic Role Usage

```bash
# Include in playbook
- hosts: satellite_servers
  roles:
    - ansible-role-satellite

# Run with ansible-playbook
ansible-playbook -i inventory satellite_playbook.yml
```

### Role Variables

```yaml
# Example configuration in group_vars or host_vars
satellite_version: "6.17"
satellite_admin_username: "admin"
satellite_admin_password: "changeme123"
satellite_organization: "Default Organization"
satellite_location: "Default Location"
```

### Available Tasks

- Satellite installation and initial setup
- Organization and location configuration
- User and permission management
- Content view and lifecycle environment setup
- Host group and activation key creation
- Repository synchronization management

## Features and Capabilities

### Core Features

- Automated Satellite installation
- Configuration management for Satellite components
- User and organization management
- Repository and content management
- Host registration and management
- Backup and restore operations

### Installation Management

- Pre-installation system preparation
- Package installation and configuration
- Service management and monitoring
- SSL certificate management
- Database configuration and optimization

### Content Management

- Repository creation and synchronization
- Content view management
- Lifecycle environment configuration
- Activation key management
- Package and errata management

### Advanced Features

- High availability configuration support
- Capsule server management
- Custom configuration templates
- Integration with external authentication
- Monitoring and alerting setup

## Limitations

- Requires Red Hat subscription for Satellite software
- Significant system resources required (minimum 20GB RAM recommended)
- Network connectivity required for repository synchronization
- May require specific firewall configurations
- Installation time can be substantial depending on content

## Getting Help

### Documentation

- Check defaults/main.yml for available variables
- Review tasks/ directory for detailed implementation
- Examine templates/ for configuration file examples
- Check meta/main.yml for role dependencies

### Support Resources

- Red Hat Satellite documentation for feature details
- Ansible role documentation for usage examples
- Check vars/ directory for version-specific configurations
- Review tests/ directory for example implementations

### Common Issues

- System resource requirements: Ensure sufficient RAM, CPU, and storage
- Network connectivity: Verify access to Red Hat repositories
- Subscription management: Ensure valid Red Hat subscriptions
- Firewall configuration: Check required port accessibility
- Service dependencies: Verify all required services are available

## Legal Disclaimer

This software is provided "as is" without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and non-infringement. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability, whether in an action of contract, tort, or otherwise, arising from, out of, or in connection with the software or the use or other dealings in the software.

Use this software at your own risk. No warranty is implied or provided.

**By Shadd**
