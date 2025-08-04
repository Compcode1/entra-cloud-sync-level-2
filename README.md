Entra Cloud Sync Level 2 – Technical Configuration
This project builds on the foundational Level 1 scenario: enabling Microsoft Entra Cloud Sync for a small business with an existing on-premises Active Directory. While Level 1 focused on business fit and general architecture, Level 2 documents the technical steps required to deploy the synchronization agent and securely establish identity synchronization between on-prem and cloud.

🔧 Project Scope (Level 2)
Focus: Agent installation, permissions, and initial sync validation

Reuses Level 1 scenario (Acme Finance Group) for continuity

Demonstrates technical viability of lightweight hybrid identity without custom rules or advanced flows

✅ Key Configuration Steps
Install Cloud Sync Agent

Requirements: .NET Framework 4.7.2+, Windows Server with access to domain controllers

Installation via lightweight wizard downloaded from Microsoft Entra Admin Center

Grant Directory Permissions

Admin grants delegated access using the provisioning wizard

Domain acme.local is successfully authorized for synchronization

Define Organizational Units (OUs)

Admin selects which on-prem OUs will sync to Entra ID

Example: sync only Accounting and Support user groups

Enable Initial Sync

Sync status is verified via Entra ID portal

Optional: test sign-in with synced user to confirm result

🧭 Roadmap Context
This project is Level 2 of a five-level roadmap:

Level 1 – Business Fit & Orientation (completed)

Level 2 – Technical Configuration (this project)

Level 3 – Custom Use Cases (coming next)

Level 4 – Monitoring, Troubleshooting, and Health

Level 5 – Migration Planning & Advanced Integration

🔗 Related Projects
Level 1: Initial Hybrid Identity Integration via Microsoft Entra Cloud Sync
