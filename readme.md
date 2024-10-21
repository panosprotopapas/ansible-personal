# Debian 12 Automation Playbook

This repository contains an Ansible playbook designed to automate the setup of a fresh Debian 12 installation. While the playbook covers many essential tasks, there are still areas that require manual intervention. Below are some of the current limitations and future improvements planned for this project.

## Current Limitations

- **Software Version Pinning**: Certain software packages are pinned to specific versions rather than the latest available. This may cause them to become outdated and potentially unusable over time (e.g., Tuxedo software).
- **Manual Installations**: Several software packages and configurations still need to be installed manually by the user.
- **Gnome Settings**: Many Gnome settings are not automated and must be configured manually by the user.
- **Gnome Extensions**: All Gnome extensions need to be installed manually. An existing Ansible role for this purpose was found to be ineffective.

## Features

Despite the limitations, the playbook successfully automates several key tasks, including:

- **OneDrive Integration**: Automatically mounts OneDrive folders using rclone.

## Directory Structure

- **`./secrets`**: This folder is intentionally included with empty `*.example` files for reference.
