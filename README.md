# Microsoft (microsoft)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Collection of Microsoft's primary APIs and developer resources.

**APIs.json:** [https://www.microsoft.com](https://www.microsoft.com)

## Timestamps

- **Created:** 2024
- **Modified:** 2026-05-19

## APIs

### Microsoft Graph API

Unified API endpoint for accessing Microsoft 365, Windows, and Enterprise Mobility + Security services.

- **Human URL:** [https://developer.microsoft.com/en-us/graph](https://developer.microsoft.com/en-us/graph)
- **Base URL:** `https://graph.microsoft.com`

#### Tags

- Azure AD
- Office 365
- OneDrive
- Outlook
- Teams

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/graph/overview)
- [OpenAPI](https://learn.microsoft.com/en-us/graph/api/overview) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Authentication](https://learn.microsoft.com/en-us/graph/auth/)
- [S D Ks](https://learn.microsoft.com/en-us/graph/sdks/sdks-overview)
- [Graph  Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer)
- [Changelog](https://learn.microsoft.com/en-us/graph/whats-new-overview)
- [Getting Started](https://learn.microsoft.com/en-us/graph/use-the-api)
- [OpenAPI](openapi/microsoft-graph-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/microsoft-graph.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-graph.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/microsoft-graph-user-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/microsoft-graph-group-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Azure REST API

REST APIs for managing Azure resources and services.

- **Human URL:** [https://learn.microsoft.com/en-us/rest/api/azure/](https://learn.microsoft.com/en-us/rest/api/azure/)
- **Base URL:** `https://management.azure.com`

#### Tags

- Azure
- Cloud
- Infrastructure
- Resources

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/rest/api/azure/)
- [API Reference](https://learn.microsoft.com/en-us/rest/api/?view=Azure)
- [Authentication](https://learn.microsoft.com/en-us/azure/active-directory/develop/)
- [S D Ks](https://azure.microsoft.com/en-us/downloads/)
- [Pricing](https://azure.microsoft.com/en-us/pricing/)
- [OpenAPI](openapi/microsoft-azure-rest-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/microsoft-azure-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-azure-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/microsoft-azure-resource-group-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Azure OpenAI Service API

Access to OpenAI's powerful language models through Azure.

- **Human URL:** [https://azure.microsoft.com/en-us/products/ai-services/openai-service](https://azure.microsoft.com/en-us/products/ai-services/openai-service)
- **Base URL:** `https://{resource-name}.openai.azure.com`

#### Tags

- AI
- GPT
- Machine Learning
- OpenAI

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/azure/ai-services/openai/)
- [API Reference](https://learn.microsoft.com/en-us/azure/ai-services/openai/reference)
- [Quickstart](https://learn.microsoft.com/en-us/azure/ai-services/openai/quickstart)
- [Pricing](https://azure.microsoft.com/en-us/pricing/details/cognitive-services/openai-service/)
- [Authentication](https://learn.microsoft.com/en-us/azure/ai-services/openai/how-to/managed-identity)
- [OpenAPI](openapi/microsoft-azure-openai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/microsoft-azure-openai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-azure-openai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Azure Cognitive Services API

APIs for vision, speech, language, and decision-making AI capabilities.

- **Human URL:** [https://azure.microsoft.com/en-us/products/ai-services/](https://azure.microsoft.com/en-us/products/ai-services/)
- **Base URL:** `https://{region}.api.cognitive.microsoft.com`

#### Tags

- AI
- Computer Vision
- Language
- Machine Learning
- Speech

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/azure/ai-services/)
- [API Reference](https://learn.microsoft.com/en-us/rest/api/cognitiveservices/)
- [Pricing](https://azure.microsoft.com/en-us/pricing/details/cognitive-services/)
- [S D Ks](https://learn.microsoft.com/en-us/azure/ai-services/cognitive-services-apis-create-account-client-library)
- [OpenAPI](openapi/microsoft-azure-cognitive-services-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/microsoft-azure-cognitive-services.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-azure-cognitive-services.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Microsoft Teams API

Build apps and bots for Microsoft Teams.

- **Human URL:** [https://developer.microsoft.com/en-us/microsoft-teams](https://developer.microsoft.com/en-us/microsoft-teams)
- **Base URL:** `https://graph.microsoft.com/v1.0/teams`

#### Tags

- Chat
- Collaboration
- Messaging
- Teams

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/microsoftteams/platform/)
- [API Reference](https://learn.microsoft.com/en-us/graph/teams-concept-overview)
- [App  Templates](https://learn.microsoft.com/en-us/microsoftteams/platform/samples/app-templates)
- [S D Ks](https://learn.microsoft.com/en-us/microsoftteams/platform/get-started/get-started-overview)
- [OpenAPI](openapi/microsoft-teams-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/microsoft-teams.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-teams.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/microsoft-teams-team-schema.json) — [JSON Schema](https://json-schema.org/specification)

### OneDrive API

Access and manage files stored in OneDrive and SharePoint.

- **Human URL:** [https://developer.microsoft.com/en-us/onedrive](https://developer.microsoft.com/en-us/onedrive)
- **Base URL:** `https://graph.microsoft.com/v1.0/me/drive`

#### Tags

- Files
- OneDrive
- SharePoint
- Storage

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/onedrive/developer/)
- [API Reference](https://learn.microsoft.com/en-us/onedrive/developer/rest-api/)
- [Samples](https://github.com/OneDrive/samples)
- [OpenAPI](openapi/microsoft-onedrive-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/microsoft-onedrive.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-onedrive.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/microsoft-drive-item-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Power Platform API

APIs for Power Apps, Power Automate, and Power BI.

- **Human URL:** [https://learn.microsoft.com/en-us/power-platform/](https://learn.microsoft.com/en-us/power-platform/)
- **Base URL:** `https://api.powerplatform.com`

#### Tags

- Automation
- Business Intelligence
- Low Code
- Power Apps

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/power-platform/admin/programmability-overview)
- [Power  Apps  A P I](https://learn.microsoft.com/en-us/power-apps/developer/data-platform/webapi/overview)
- [Power  Automate  A P I](https://learn.microsoft.com/en-us/power-automate/web-api)
- [OpenAPI](openapi/microsoft-power-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/microsoft-power-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-power-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bing Search APIs

Integrate Bing search capabilities into applications.

- **Human URL:** [https://www.microsoft.com/en-us/bing/apis/bing-web-search-api](https://www.microsoft.com/en-us/bing/apis/bing-web-search-api)
- **Base URL:** `https://api.bing.microsoft.com/v7.0`

#### Tags

- Bing
- Image Search
- Search
- Web Search

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/bing/search-apis/)
- [API Reference](https://learn.microsoft.com/en-us/bing/search-apis/bing-web-search/reference/endpoints)
- [Pricing](https://www.microsoft.com/en-us/bing/apis/pricing)
- [OpenAPI](openapi/microsoft-bing-search-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/microsoft-bing-search.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-bing-search.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### SharePoint REST API

REST service for remotely interacting with SharePoint data using standard REST and OData web protocol standards.

- **Human URL:** [https://learn.microsoft.com/en-us/sharepoint/dev/sp-add-ins/get-to-know-the-sharepoint-rest-service](https://learn.microsoft.com/en-us/sharepoint/dev/sp-add-ins/get-to-know-the-sharepoint-rest-service)
- **Base URL:** `https://{tenant}.sharepoint.com/_api`

#### Tags

- Collaboration
- Content Management
- Documents
- SharePoint

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/sharepoint/dev/sp-add-ins/get-to-know-the-sharepoint-rest-service)
- [API Reference](https://learn.microsoft.com/en-us/sharepoint/dev/sp-add-ins/complete-basic-operations-using-sharepoint-rest-endpoints)
- [Getting Started](https://learn.microsoft.com/en-us/sharepoint/dev/apis/sharepoint-rest-graph)
- [Microsoft  Graph  Integration](https://learn.microsoft.com/en-us/graph/sharepoint-concept-overview)
- [OpenAPI](openapi/microsoft-sharepoint-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/microsoft-sharepoint.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-sharepoint.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Power BI REST API

REST APIs for embedded analytics, administration, governance, and content management in Power BI.

- **Human URL:** [https://learn.microsoft.com/en-us/power-bi/developer/](https://learn.microsoft.com/en-us/power-bi/developer/)
- **Base URL:** `https://api.powerbi.com/v1.0/myorg`

#### Tags

- Analytics
- Business Intelligence
- Dashboards
- Reports

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/power-bi/developer/)
- [API Reference](https://learn.microsoft.com/en-us/rest/api/power-bi/)
- [S D Ks](https://learn.microsoft.com/en-us/power-bi/developer/embedded/)
- [Authentication](https://learn.microsoft.com/en-us/power-bi/developer/embedded/register-app)
- [OpenAPI](openapi/microsoft-power-bi-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/microsoft-power-bi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-power-bi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Azure DevOps REST API

REST APIs for managing Azure DevOps Services including projects, pipelines, repositories, and work items.

- **Human URL:** [https://learn.microsoft.com/en-us/rest/api/azure/devops/](https://learn.microsoft.com/en-us/rest/api/azure/devops/)
- **Base URL:** `https://dev.azure.com/{organization}/_apis`

#### Tags

- CI/CD
- DevOps
- Git
- Pipelines
- Work Items

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/rest/api/azure/devops/)
- [Getting Started](https://learn.microsoft.com/en-us/azure/devops/integrate/how-to/call-rest-api)
- [Authentication](https://learn.microsoft.com/en-us/azure/devops/integrate/get-started/authentication/authentication-guidance)
- [Samples](https://learn.microsoft.com/en-us/azure/devops/integrate/get-started/rest/samples)
- [OpenAPI](openapi/microsoft-azure-devops-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/microsoft-azure-devops.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-azure-devops.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Dynamics 365 REST API

REST APIs for Dynamics 365 business applications including Customer Engagement, Business Central, and Dataverse.

- **Human URL:** [https://learn.microsoft.com/en-us/rest/dynamics365/](https://learn.microsoft.com/en-us/rest/dynamics365/)
- **Base URL:** `https://{org}.api.crm.dynamics.com/api/data/v9.2`

#### Tags

- Business Applications
- CRM
- Dynamics
- ERP

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/rest/dynamics365/)
- [API Reference](https://learn.microsoft.com/en-us/power-apps/developer/data-platform/webapi/reference/about)
- [Getting Started](https://learn.microsoft.com/en-us/power-apps/developer/data-platform/webapi/overview)
- [Authentication](https://learn.microsoft.com/en-us/power-apps/developer/data-platform/authenticate-oauth)
- [OpenAPI](openapi/microsoft-dynamics-365-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/microsoft-dynamics-365.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-dynamics-365.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LinkedIn API

APIs for LinkedIn integrations covering consumer, marketing, sales, talent, learning, and compliance solutions.

- **Human URL:** [https://developer.linkedin.com/](https://developer.linkedin.com/)
- **Base URL:** `https://api.linkedin.com/v2`

#### Tags

- Marketing
- Professional Network
- Recruiting
- Social

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/linkedin/)
- [Authentication](https://learn.microsoft.com/en-us/linkedin/shared/authentication/getting-access)
- [API Reference](https://learn.microsoft.com/en-us/linkedin/shared/api-guide/concepts)
- [S D Ks](https://learn.microsoft.com/en-us/linkedin/shared/development-resources/api-clients)
- [OpenAPI](openapi/microsoft-linkedin-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Azure Communication Services API

Multichannel communication APIs for adding voice, video, chat, SMS, and email to applications.

- **Human URL:** [https://learn.microsoft.com/en-us/azure/communication-services/](https://learn.microsoft.com/en-us/azure/communication-services/)
- **Base URL:** `https://{resource}.communication.azure.com`

#### Tags

- Chat
- Communication
- Email
- SMS
- Video
- Voice

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/azure/communication-services/)
- [API Reference](https://learn.microsoft.com/en-us/rest/api/communication/)
- [S D Ks](https://learn.microsoft.com/en-us/azure/communication-services/concepts/sdk-options)
- [Pricing](https://azure.microsoft.com/en-us/products/communication-services/#pricing)
- [Git Hub](https://github.com/Azure/Communication)
- [OpenAPI](openapi/microsoft-azure-communication-services-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/microsoft-azure-communication-services.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-azure-communication-services.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Microsoft Entra ID API

APIs for identity and access management including user authentication, authorization, and directory services via Microsoft Graph.

- **Human URL:** [https://learn.microsoft.com/en-us/entra/identity-platform/](https://learn.microsoft.com/en-us/entra/identity-platform/)
- **Base URL:** `https://graph.microsoft.com/v1.0`

#### Tags

- Authentication
- Authorization
- Directory
- Identity
- Security

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/entra/identity-platform/)
- [API Reference](https://learn.microsoft.com/en-us/graph/identity-network-access-overview)
- [Getting Started](https://learn.microsoft.com/en-us/entra/identity-platform/quickstart-register-app)
- [Authentication](https://learn.microsoft.com/en-us/entra/identity-platform/v2-overview)
- [OpenAPI](openapi/microsoft-entra-id-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/microsoft-entra-id.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-entra-id.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Microsoft Outlook API

APIs for integrating with Outlook mail, calendar, and contacts through Microsoft Graph.

- **Human URL:** [https://developer.microsoft.com/en-us/outlook](https://developer.microsoft.com/en-us/outlook)
- **Base URL:** `https://graph.microsoft.com/v1.0/me`

#### Tags

- Calendar
- Contacts
- Email
- Outlook

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/outlook/)
- [Mail  A P I  Reference](https://learn.microsoft.com/en-us/graph/outlook-mail-concept-overview)
- [Calendar  A P I  Reference](https://learn.microsoft.com/en-us/graph/outlook-calendar-concept-overview)
- [Getting Started](https://learn.microsoft.com/en-us/outlook/rest/get-started)
- [OpenAPI](openapi/microsoft-outlook-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/microsoft-outlook.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-outlook.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Microsoft Intune API

APIs for managing devices, apps, and compliance policies through Microsoft Graph for enterprise mobility management.

- **Human URL:** [https://learn.microsoft.com/en-us/graph/intune-concept-overview](https://learn.microsoft.com/en-us/graph/intune-concept-overview)
- **Base URL:** `https://graph.microsoft.com/v1.0`

#### Tags

- Compliance
- Device Management
- Endpoint Management
- Mobile

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/graph/intune-concept-overview)
- [API Reference](https://learn.microsoft.com/en-us/graph/api/resources/intune-graph-overview)
- [Authentication](https://learn.microsoft.com/en-us/intune/intune-service/developer/intune-graph-apis)
- [S D Ks](https://learn.microsoft.com/en-us/intune/intune-service/developer/app-sdk-get-started)
- [OpenAPI](openapi/microsoft-intune-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/microsoft-intune.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-intune.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/microsoft-managed-device-schema.json) — [JSON Schema](https://json-schema.org/specification)

## Common Properties

- [Developer  Portal](https://developer.microsoft.com/)
- [Azure  Portal](https://portal.azure.com)
- [Status Page](https://status.azure.com/)
- [Support](https://support.microsoft.com/)
- [Privacy Policy](https://privacy.microsoft.com/)
- [Terms of Service](https://www.microsoft.com/en-us/legal/terms-of-use)
- [Blog](https://devblogs.microsoft.com/)
- [Authentication](https://learn.microsoft.com/en-us/entra/identity-platform/)
- [Sign Up](https://developer.microsoft.com/en-us/microsoft-365/dev-program)
- [Forum](https://learn.microsoft.com/en-us/answers/)
- [Pricing](https://azure.microsoft.com/en-us/pricing/calculator/)
- [Git Hub](https://github.com/microsoft)
- [JSON-LD](json-ld/microsoft-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/microsoft-graph-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON Schema](json-schema/microsoft-graph-user-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/microsoft-graph-group-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/microsoft-azure-resource-group-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/microsoft-teams-team-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/microsoft-drive-item-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/microsoft-managed-device-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Features](undefined)
- [Integrations](https://www.microsoft.com/en-us/marketplace)

## Maintainers

**Email:** kin@apievangelist.com
**URL:** https://apievangelist.com
