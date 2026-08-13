# AZ-104 Microsoft Azure Administrator — Hands-On Labs

> **Read → Build → Verify → Break → Troubleshoot → Document → Repeat → Recall**

This repository is a practical AZ-104 learning environment built around Microsoft's official AZ-104 lab sequence. It is designed to record **what I can actually do**, not merely what I have read.

The repository combines:

- Hands-on laboratory workbook
- Personal Azure administration notebook
- AZ-104 revision guide
- Troubleshooting journal
- Screenshot-based practical reference
- Azure CLI and PowerShell command library
- GitHub portfolio of practical Azure administration skills

## Source of truth

The official Microsoft lab portal is the baseline for lab numbering, objectives, tasks and procedures:

- [Official AZ-104 lab portal](https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/)
- [Official MicrosoftLearning repository](https://github.com/MicrosoftLearning/AZ-104-MicrosoftAzureAdministrator)

Microsoft's current hosted lab directory contains Labs 01, 02a, 02b, 03, 04, 05, 06, 07, 08, 09a, 09b, 09c, 10 and 11. citeturn0search0

**Important:** this repository intentionally separates the official procedure from personal practice notes. Microsoft lab instructions can change as Azure changes, so the official lab remains authoritative. citeturn0search1turn0search2

## 🧠 Building Azure Muscle Memory

Every lab follows:

```text
Learn
  ↓
Build
  ↓
Verify
  ↓
Break / Troubleshoot
  ↓
Document
  ↓
Repeat
  ↓
Recall
```

The goal is to reach the point where I can perform the administration task without opening the instructions, explain why the configuration matters, verify the result, and troubleshoot failure.

## 🗺️ AZ-104 Lab Roadmap

| Lab | Topic | Status | Last Practiced | Confidence |
|---|---|---|---|---|
| 01 | Microsoft Entra ID Identities | ⬜ Not Started | | ⭐☆☆☆☆ |
| 02a | Subscriptions and RBAC | ⬜ Not Started | | ⭐☆☆☆☆ |
| 02b | Azure Policy Governance | ⬜ Not Started | | ⭐☆☆☆☆ |
| 03 | ARM Templates and Bicep | ⬜ Not Started | | ⭐☆☆☆☆ |
| 04 | Virtual Networking | ⬜ Not Started | | ⭐☆☆☆☆ |
| 05 | Intersite Connectivity | ⬜ Not Started | | ⭐☆☆☆☆ |
| 06 | Network Traffic Management | ⬜ Not Started | | ⭐☆☆☆☆ |
| 07 | Azure Storage | ⬜ Not Started | | ⭐☆☆☆☆ |
| 08 | Virtual Machines | ⬜ Not Started | | ⭐☆☆☆☆ |
| 09a | Web Apps | ⬜ Not Started | | ⭐☆☆☆☆ |
| 09b | Azure Container Instances | ⬜ Not Started | | ⭐☆☆☆☆ |
| 09c | Azure Container Apps | ⬜ Not Started | | ⭐☆☆☆☆ |
| 10 | Data Protection | ⬜ Not Started | | ⭐☆☆☆☆ |
| 11 | Monitoring | ⬜ Not Started | | ⭐☆☆☆☆ |

### Status values

- ⬜ Not Started
- 🟡 In Progress
- 🟢 Completed
- 🔁 Repeated
- ⭐ Exam Ready

Do not mark a lab complete because it was read. Completion means the hands-on workflow was performed and verified.

## How I use this repository

1. Open the official Microsoft lab.
2. Read the objective and scenario.
3. Open the corresponding repository README.
4. Perform the lab in Azure.
5. Capture meaningful screenshots.
6. Store screenshots under that lab's `images/` directory.
7. Record commands used.
8. Record mistakes and fixes.
9. Complete the verification section.
10. Write AZ-104 exam notes.
11. Clean up billable resources.
12. Repeat the lab later without instructions.
13. Update confidence.

## 📸 Screenshot strategy

Screenshots are evidence of practice, not decoration.

Use predictable names such as:

```text
01-task-01-entra-overview.png
02-task-01-create-user.png
03-task-02-create-group.png
```

Reference them with relative paths:

```markdown
![Azure Portal - Example](./images/01-task-01-entra-overview.png)
```

Only screenshots captured from my own practice environment should be committed. The repository contains Markdown placeholders, not fake images.

## 🧠 Muscle Memory Standard

A lab is approaching exam-ready when I can:

- [ ] Explain the purpose of the Azure service.
- [ ] Navigate to the service without searching for the instructions.
- [ ] Create the required resource.
- [ ] Configure the important settings.
- [ ] Verify the configuration.
- [ ] Explain common failure modes.
- [ ] Troubleshoot the configuration.
- [ ] Perform the task with Azure CLI where appropriate.
- [ ] Perform the task with Azure PowerShell where appropriate.
- [ ] Explain the AZ-104 exam concepts.
- [ ] Reproduce the core workflow from memory.

## ⭐ Confidence scale

| Rating | Meaning |
|---|---|
| ⭐☆☆☆☆ | I need the instructions |
| ⭐⭐☆☆☆ | I understand the concept |
| ⭐⭐⭐☆☆ | I can complete it with minimal help |
| ⭐⭐⭐⭐☆ | I can complete it independently |
| ⭐⭐⭐⭐⭐ | I can explain and troubleshoot it |

Confidence measures practical ability, not familiarity with the documentation.

## Repository map

```text
00-az104-study-roadmap/   Study plan and progression
01-... through 11-...     Hands-on labs
exam-notes/                High-value revision notes
troubleshooting/           Cross-lab troubleshooting knowledge base
scripts/                   CLI and PowerShell command library
templates/                 Reusable documentation templates
```

## Git workflow

Keep commits small and meaningful:

```bash
git add .
git commit -m "Complete Lab 01 Entra ID identities"
git push
```

Examples:

```bash
git commit -m "Add Lab 04 networking practice screenshots"
git commit -m "Document Lab 05 peering troubleshooting"
git commit -m "Update Lab 07 storage exam notes"
```

## 🔐 Security — never commit secrets

Never commit:

- Passwords
- Client secrets
- API keys
- Access keys
- Private keys
- Connection strings
- SAS tokens
- Tenant secrets
- Subscription credentials

Use placeholders:

```text
<YOUR_SUBSCRIPTION_ID>
<YOUR_TENANT_ID>
<YOUR_RESOURCE_GROUP>
<YOUR_STORAGE_ACCOUNT>
```

Review staged changes before pushing:

```bash
git diff --cached
```

## 🧹 Cleanup

Azure resources can incur charges. Every lab should identify resources that can be deleted after practice.

Do not assume that deleting one resource automatically deletes all related resources. Verify the dependency tree first.

## 🎯 The end state

The repository should eventually become an Azure Administrator's personal field manual:

```text
Read the Lab
     ↓
Perform the Lab
     ↓
Capture the Configuration
     ↓
Capture Screenshots
     ↓
Document Mistakes
     ↓
Understand the Why
     ↓
Repeat Without Instructions
     ↓
Explain It
     ↓
Troubleshoot It
     ↓
Become Exam Ready
```

## License / attribution

This repository is a personal learning companion to Microsoft's AZ-104 labs. Microsoft lab procedures remain the property of their respective source and should be followed from the official Microsoft Learning repository/portal. This repository adds personal practice structure, observations, screenshots, troubleshooting records and revision notes.

## Official resources

- [Microsoft AZ-104 hosted labs](https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/)
- [MicrosoftLearning AZ-104 repository](https://github.com/MicrosoftLearning/AZ-104-MicrosoftAzureAdministrator)
