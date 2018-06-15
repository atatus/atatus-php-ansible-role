# Ansible Role: Atatus PHP Agent

Installs Atatus PHP Agent, PHP Performance Monitoring.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

Workspace where certain files will be downloaded and adjusted prior to agent installation, if needed.

    workspace: /root

`atatus_api_key` contains Project API Key.

`atatus_ini_file` defines where `atatus.ini` is placed and used for updating the API Key.

`php_service_name` is the name of PHP Server. It can be apache2, httpd or php-fpm

`linux_distribution` defines linux distribution where you are going to install PHP agent.

`atatus_php_version` is the Atatus PHP Agent version.

## Dependencies

None.

## Example Playbook

    - hosts: servers
      roles:
        - { role: atatus-php-ansible-role }
