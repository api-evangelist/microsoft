# Microsoft Graph — Conceptual GraphQL Schema

## Overview

Microsoft Graph is the unified REST/OData gateway to Microsoft 365, Azure Active Directory, Intune, and related services. While Microsoft does not publish an official GraphQL endpoint, the resource model maps cleanly to GraphQL types. This document describes a conceptual GraphQL layer over Microsoft Graph, covering M365 productivity, Azure AD identity, DevOps, Security, and Intune device-management domains.

- **Source API**: Microsoft Graph API (`https://graph.microsoft.com/v1.0`)
- **GitHub (SDK & samples)**: https://github.com/microsoftgraph
- **Docs**: https://learn.microsoft.com/en-us/graph/api/resources/
- **Graph Explorer**: https://developer.microsoft.com/en-us/graph/graph-explorer
- **Schema file**: `microsoft-schema.graphql`

---

## Domain Coverage

### M365 Productivity
User, Group, Team, Channel, ChannelMessage, Calendar, Event, Attendee, Contact, MailFolder, Message, Attachment, Drive, DriveItem, Site, SharePointList, ListItem, Planner, PlannerPlan, PlannerTask, PlannerBucket, TodoTaskList, TodoTask, OneNoteNotebook, OneNotePage, OneNoteSection

### Azure AD / Entra ID
Application, ServicePrincipal, OAuth2PermissionGrant, AppRole, AppRoleAssignment, DirectoryRole, DirectoryRoleAssignment, ConditionalAccessPolicy, ManagedIdentity, Organization, Domain, SubscribedSku, License, AssignedLicense

### DevOps
Repository, PullRequest, PullRequestReviewer, PipelineRun, Build, Release, TestPlan, TestCase, WorkItem, WorkItemComment

### Security
SecurityAlert, SecureScore, SecureScoreControlProfile, ThreatIntelligence, IdentityRiskEvent, RiskyUser, RiskySignIn, AuditLog, AuditLogRecord, SignInLog, SignInRecord

### Intune
ManagedDevice, DeviceConfiguration, DeviceCompliancePolicy, MobileApp, AppConfiguration, DeviceEnrollmentConfiguration, DetectedApp

---

## Root Query Fields

| Field | Return Type | Description |
|-------|-------------|-------------|
| `me` | `User` | Authenticated user |
| `user(id: ID!)` | `User` | User by ID or UPN |
| `users` | `[User]` | All users in tenant |
| `group(id: ID!)` | `Group` | Group by ID |
| `groups` | `[Group]` | All groups |
| `team(id: ID!)` | `Team` | Team by ID |
| `teams` | `[Team]` | All Teams in tenant |
| `site(id: ID!)` | `Site` | SharePoint site |
| `sites` | `[Site]` | All sites |
| `drive(id: ID!)` | `Drive` | Drive by ID |
| `application(id: ID!)` | `Application` | App registration |
| `applications` | `[Application]` | All app registrations |
| `servicePrincipal(id: ID!)` | `ServicePrincipal` | Service principal |
| `organization` | `Organization` | Tenant organization |
| `domains` | `[Domain]` | Verified domains |
| `conditionalAccessPolicies` | `[ConditionalAccessPolicy]` | CA policies |
| `securityAlerts` | `[SecurityAlert]` | Security alerts |
| `secureScore` | `SecureScore` | Latest secure score |
| `riskyUsers` | `[RiskyUser]` | At-risk users |
| `auditLogs` | `[AuditLogRecord]` | Audit log records |
| `signInLogs` | `[SignInRecord]` | Sign-in logs |
| `managedDevices` | `[ManagedDevice]` | Intune managed devices |
| `mobileApps` | `[MobileApp]` | Intune mobile apps |
| `workItem(id: ID!)` | `WorkItem` | Azure DevOps work item |
| `repository(id: ID!)` | `Repository` | DevOps repository |

---

## Root Mutation Fields

| Field | Description |
|-------|-------------|
| `createUser(input: CreateUserInput!)` | Create a new user |
| `updateUser(id: ID!, input: UpdateUserInput!)` | Update user properties |
| `deleteUser(id: ID!)` | Delete a user |
| `createGroup(input: CreateGroupInput!)` | Create a group |
| `addGroupMember(groupId: ID!, userId: ID!)` | Add member to group |
| `removeGroupMember(groupId: ID!, userId: ID!)` | Remove member from group |
| `createTeam(input: CreateTeamInput!)` | Provision a new Team |
| `createChannel(teamId: ID!, input: CreateChannelInput!)` | Add channel to Team |
| `sendChannelMessage(teamId: ID!, channelId: ID!, input: MessageInput!)` | Post a message |
| `createEvent(calendarId: ID!, input: CreateEventInput!)` | Create calendar event |
| `updateEvent(id: ID!, input: UpdateEventInput!)` | Update event |
| `deleteEvent(id: ID!)` | Delete event |
| `sendMail(input: SendMailInput!)` | Send an email via Graph |
| `createPlannerPlan(input: CreatePlannerPlanInput!)` | Create Planner plan |
| `createPlannerTask(input: CreatePlannerTaskInput!)` | Create Planner task |
| `createTodoTask(listId: ID!, input: CreateTodoTaskInput!)` | Create To Do task |
| `createApplication(input: CreateApplicationInput!)` | Register application |
| `assignLicense(userId: ID!, input: AssignLicenseInput!)` | Assign M365 license |
| `createConditionalAccessPolicy(input: CreateConditionalAccessPolicyInput!)` | Create CA policy |
| `updateManagedDevice(id: ID!, input: UpdateManagedDeviceInput!)` | Update Intune device |
| `wipeDevice(id: ID!)` | Remote wipe Intune device |

---

## Type Descriptions

### User
Core identity object. Covers profile fields (displayName, mail, jobTitle, department, officeLocation), account state (accountEnabled), assigned licenses, group memberships, manager chain, owned applications, calendar, mailbox, drives, and todo lists.

### Group
Microsoft 365 group or security group. Includes members, owners, transitive members, and linked Team/SharePoint site.

### Team and Channel
Teams collaboration surface. Team wraps a Group. Channels carry messages, tabs, and members. ChannelMessage supports replies (threaded) and reactions.

### Calendar and Event
Outlook calendar resources. Events have attendees, recurrence patterns, online-meeting details, and attachments.

### Message and MailFolder
Outlook mail. Messages have from/toRecipients/ccRecipients, body (text or HTML), attachments, and flag status.

### Drive and DriveItem
OneDrive/SharePoint file storage. DriveItem covers files, folders, and OneNote notebooks. Supports sharing links and permissions.

### Site, SharePointList, ListItem
SharePoint sites surface subsites, drive, and lists. ListItem holds column values as a dynamic fields map.

### Planner
Planner plans contain buckets; buckets contain tasks. PlannerTask tracks assignment, progress, due dates, and checklist.

### TodoTaskList and TodoTask
Microsoft To Do. Tasks support due dates, reminders, recurrence, and linked resources.

### OneNoteNotebook, OneNoteSection, OneNotePage
Hierarchical OneNote structure. Pages carry HTML content.

### Application and ServicePrincipal
Entra ID app registrations and enterprise apps. Include OAuth2 permission grants, app roles, and assigned service principals.

### ConditionalAccessPolicy
Zero-Trust access policy. Defines conditions (users, apps, locations, device state) and grant/session controls.

### ManagedIdentity
System-assigned or user-assigned managed identity for Azure resources.

### Organization, Domain, SubscribedSku
Tenant-level identity metadata, verified domains, and M365 license SKUs.

### SecurityAlert
Unified alert from Microsoft Defender, Sentinel, and partner products.

### SecureScore
Tenant-level security posture score with control-level breakdown.

### RiskyUser and RiskySignIn
Entra ID Identity Protection risk signals. Tracks risk level, state, and history.

### AuditLogRecord and SignInRecord
Entra ID audit and sign-in activity. Supports filtering by date range, user, app, and category.

### ManagedDevice
Intune-enrolled device. Tracks OS, compliance state, last check-in, encryption, and assigned user.

### DeviceConfiguration and DeviceCompliancePolicy
Intune configuration profiles and compliance rules assigned to device groups.

### MobileApp and AppConfiguration
Intune mobile app lifecycle management and per-app configuration policies.

### Repository, PullRequest, Build, Release, PipelineRun
Azure DevOps entities. Repository links to pull requests. PullRequest tracks reviewers and status. Build and PipelineRun cover CI execution. Release manages deployment stages.

### WorkItem
Azure Boards work item (Epic, Feature, User Story, Task, Bug). Carries fields, state, assigned user, and comments.

---

## Authentication

All Microsoft Graph queries require OAuth 2.0 Bearer tokens from the Microsoft identity platform (`login.microsoftonline.com`). Permissions are granted as delegated (user context) or application (daemon) scopes.

Common scopes:
- `User.Read`, `User.ReadWrite.All`
- `Group.Read.All`, `Team.ReadBasic.All`
- `Mail.Read`, `Calendars.ReadWrite`
- `Files.ReadWrite.All`, `Sites.Read.All`
- `DeviceManagementManagedDevices.Read.All`
- `SecurityEvents.Read.All`, `AuditLog.Read.All`

---

## References

- Microsoft Graph overview: https://learn.microsoft.com/en-us/graph/overview
- Resource type index: https://learn.microsoft.com/en-us/graph/api/resources/
- Graph SDK (GitHub): https://github.com/microsoftgraph
- Graph Explorer: https://developer.microsoft.com/en-us/graph/graph-explorer
- Permissions reference: https://learn.microsoft.com/en-us/graph/permissions-reference
