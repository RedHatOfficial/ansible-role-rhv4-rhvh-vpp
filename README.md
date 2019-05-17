VPP - Protection Profile for Virtualization v. 1.0 for Red Hat Virtualization Hypervisor (RHVH)
=========

[![Build Status](https://travis-ci.org/RedHatOfficial/ansible-role-rhv4-rhvh-vpp.svg?branch=master)](https://travis-ci.org/RedHatOfficial/ansible-role-rhv4-rhvh-vpp)
[![Ansible Role](https://img.shields.io/ansible/role/40487.svg)](https://galaxy.ansible.com/RedHatOfficial/rhv4-rhvh-vpp)
[![GitHub release](https://img.shields.io/github/release/RedHatOfficial/ansible-role-rhv4-rhvh-vpp.svg)](https://github.com/RedHatOfficial/ansible-role-rhv4-rhvh-vpp/releases/latest)

Ansible Role for VPP - Protection Profile for Virtualization v. 1.0 for Red Hat Virtualization Hypervisor (RHVH)  

Profile Description:  
This compliance profile reflects the core set of security  
related configuration settings for deployment of Red Hat Virtualization  
Hypervisor (RHVH) 4.x into U.S. Defense, Intelligence, and Civilian agencies.  
Development partners and sponsors include the U.S. National Institute  
of Standards and Technology (NIST), U.S. Department of Defense,  
the National Security Agency, and Red Hat.  
  
This baseline implements configuration requirements from the following  
sources:  
  
- Committee on National Security Systems Instruction No. 1253 (CNSSI 1253)  
- NIST 800-53 control selections for MODERATE impact systems (NIST 800-53)  
- U.S. Government Configuration Baseline (USGCB)  
- NIAP Protection Profile for Virtualization v1.0 (VPP v1.0)  
  
For any differing configuration requirements, e.g. password lengths, the stricter  
security setting was chosen. Security Requirement Traceability Guides (RTMs) and  
sample System Security Configuration Guides are provided via the  
scap-security-guide-docs package.  
  
This profile reflects U.S. Government consensus content and is developed through  
the ComplianceAsCode project, championed by the National  
Security Agency. Except for differences in formatting to accommodate  
publishing processes, this profile mirrors ComplianceAsCode  
content as minor divergences, such as bugfixes, work through the  
consensus and release processes.  

The tasks that are used in this role are generated using OpenSCAP.
See the OpenSCAP project for more details on Ansible playbook generation at [https://github.com/OpenSCAP/openscap](https://github.com/OpenSCAP/openscap)

To submit a fix or enhancement for an Ansible task that is failing or missing,
see the ComplianceAsCode project at [https://github.com/ComplianceAsCode/content](https://github.com/ComplianceAsCode/content)

## Requirements

- Ansible version 2.5 or higher

## Role Variables

To customize the role to your liking, check out the [list of variables](vars/main.yml).

## Dependencies

N/A

## Example Playbook

Run `ansible-galaxy install RedHatOfficial.rhv4_rhvh_vpp` to
download and install the role. Then, you can use the following playbook snippet to run the Ansible role:

    - hosts: all
      roles:
         - { role: RedHatOfficial.rhv4_rhvh_vpp }

Next, check the playbook using (on the localhost) the following example:

    ansible-playbook -i "localhost," -c local --check playbook.yml

To deploy it, use (this may change configuration of your local machine!):

    ansible-playbook -i "localhost," -c local playbook.yml

## License

BSD-3-Clause

## Author Information

This Ansible remediation role has been generated from the body of security
policies developed by the ComplianceAsCode project. Please see
[https://github.com/complianceascode/content/blob/master/Contributors.md](https://github.com/complianceascode/content/blob/master/Contributors.md)
for an updated list of authors and contributors.
