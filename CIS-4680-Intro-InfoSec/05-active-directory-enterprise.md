# Lab 05 – Using Active Directory in the Enterprise

**Course:** CIS 4680 – Introduction to Information Security and Privacy

**Platform:** ACI Learning Skill Labs

## Objective
The objective of this lab is to understand how Active Directory is used in enterprise environments to manage users, computers, groups, and security policies. This lab provides hands-on experience with creating and managing Active Directory objects, configuring permissions, and implementing centralized authentication and security controls within a Windows domain environment.

## Tools & Technologies Used
| Tool | Purpose |
|------|---------|
| Windows Server | Domain Controller hosting AD DS |
| Active Directory Users and Computers (ADUC) | User, group, and OU management |
| Group Policy Management Console (GPMC) | GPO creation and linking |
| Active Directory Administrative Center (ADAC) | Modern AD management interface |
| Server Manager | Domain controller promotion |
| PowerShell (`ActiveDirectory` module) | Scripted AD administration |
| Windows Client VM | Domain-joined workstation for testing |

## Key Concepts Covered
- **Active Directory Architecture**
- **Kerberos Authentication**
- **Users, Groups, and OUs**
- **Group Policy Objects (GPOs)**

## What I Learned
- Active Directory is the central nervous system of most enterprise Windows environments controlling it means controlling the entire domain, which is why Domain Admin accounts are so heavily targeted.
- Delegation of control is a powerful least-privilege mechanism. Help Desk staff should be able to reset passwords without having Domain Admin access, and AD's delegation model enables this precisely.
- Kerberos ticket-based authentication has security implications: a compromised TGT (Golden Ticket attack) grants unlimited access across the domain.

## Real-World Application
Active Directory (AD) is widely used in enterprise environments to centrally manage users, computers, permissions, and security policies across an organization. In a real-world business setting, system administrators rely on Active Directory to simplify account management, enforce security standards, and improve operational efficiency. For example, in a healthcare organization such as an Health System, Active Directory can be used to manage thousands of employee accounts, including doctors, nurses, administrative staff, and IT personnel. Instead of configuring permissions on every individual computer, administrators can create groups within Active Directory and assign users based on their department or job role. This allows employees to access only the systems and files necessary for their work while helping protect sensitive patient information.
