# Awesome-Authentication-SSO

## Top Authentication & SSO Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Identity Federation, Passwordless Authentication & Reverse Proxy Gateways*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Authentication & SSO**. These tools enable organizations to centralize identity, enforce multi-factor authentication, and provide single sign-on across applications—from lightweight reverse proxy companions to full-featured identity and access management platforms.



**Examples** include Duo Security, Okta Verify, Microsoft Entra ID, Ping Identity, RSA SecurID, Silverfort, Beyond Identity, HYPR, Trusona, and Yubico Cloud (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, OIDC/SAML federation, and open identity infrastructure—ideal for platform engineers, security teams, and developers seeking transparent, vendor-independent authentication.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## Sector Overview & Market Dynamics

The global Identity and Access Management (IAM) and authentication market is estimated at approximately **$23B–$27B in 2025–2026** (projected to exceed $50B by the early 2030s at an ~11–13% CAGR). The market structure is **moderately concentrated at the top**—anchored by dominant enterprise cloud oligopolies (Microsoft, Cisco, Okta, and Ping/ForgeRock)—yet remains **highly fragmented across specialized niches** such as phishing-resistant passwordless MFA, hardware tokens, zero-trust device posture, and customer IAM (CIAM).

## SaaS/Hosted Platforms

| Platform | Estimated Size (Valuation / Revenue) | Starting Pricing (Paid Tiers) | Free Tier / Trial Limit | Key Focus & Features |
| :--- | :--- | :--- | :--- | :--- |
| **[Microsoft Entra ID](https://www.microsoft.com/en-us/security/business/identity-access/microsoft-entra-id)** | **~$4.0T Market Cap** (~$332B annual revenue) | **$6.00/user/month** (Entra ID P1); $9.00/user/month (P2); $12.00/user/month (Entra Suite) | **Free tier available**: up to 50,000 objects (scale to 300k with custom domain), cloud-only SSO, basic MFA defaults, self-service password change (no SLA or Conditional Access) | Cloud identity standard with SSO, Conditional Access, Entra Verified ID, and CIEM permissions management. |
| **[Duo Security (Cisco)](https://duo.com/)** | **~$450B Market Cap** (~$63B annual revenue for Cisco) | **$3.00/user/month** (Duo Essentials); $6.00/user/month (Advantage); $9.00/user/month (Premier) | **Free tier available**: up to 10 users with basic MFA, Duo Mobile app support, and unlimited administrators (excludes SSO and risk-based policies) | Widely adopted MFA platform with push notifications, TOTP, WebAuthn, device trust, adaptive authentication, and Authelia integration. |
| **[Okta](https://www.okta.com/)** | **~$24B Market Cap** (~$2.9B annual revenue) | **$6.00/user/month** (Workforce Starter; billed annually, ~$1,500/yr minimum); $14–$17+/user/month (Essentials) | **30-day free trial**: capped at 10 active users, 1 admin email, 5 Okta Workflows, and demo environment (no production SLA) | Enterprise identity cloud with SSO, Universal Directory, Adaptive MFA, Lifecycle Management, and API access management. |
| **[Ping Identity](https://www.pingidentity.com/)** | **$2.8B Acquisition Valuation** (~$800M ARR combined with ForgeRock) | **$3.00/user/month** (Workforce Essential; 5,000-user minimum commitment, ~$180k/yr floor); $6.00/user/month (Plus) | **30-day free trial**: evaluation environment access capped at 5 trial environments per org and up to 1M identities per environment | Enterprise IAM platform merged with ForgeRock; provides SSO, MFA, orchestration, API security, and AI-driven fraud/risk protection. |
| **[RSA SecurID](https://www.rsa.com/)** | **$2.1B Acquisition Valuation** (~$300M annual revenue) | **$3.00–$5.00/user/month** (ID Plus C1 Cloud); $6.00/user/month (ID Plus M1); $7.00/user/month (ID Plus E2 Hybrid) | **45-day free trial**: full ID Plus evaluation for cloud/hybrid deployments, subject to sales-managed proof-of-concept user onboarding limits | Pioneer in hardware and software MFA tokens, now providing ID Plus access management, risk-based authentication, and zero-trust security. |
| **[Beyond Identity](https://www.beyondidentity.com/)** | **$1.1B Valuation** (Series C unicorn; ~$38M ARR) | **$6.00/user/month** (Workforce Zero Trust); CIAM starting at **$0.01/MAU/month** | **Free tier available**: core passwordless MFA for unlimited users without time expiration; enterprise advanced device trust requires a paid tier | Completely passwordless authentication with device-bound credentials, continuous risk posture checks, and phishing-resistant MFA. |
| **[Silverfort](https://www.silverfort.com/)** | **$1.0B Valuation** (Series D unicorn) | **~£5.00–£40.00/user/month** via G-Cloud framework tiers (Core/Plus/Advanced/Enterprise; typical custom contract base) | **14-day evaluation / PoC**: sales-guided enterprise proof-of-concept and identity security posture risk assessment (no self-serve free plan) | Agentless/proxyless unified identity protection extending MFA and ITDR across legacy systems, Active Directory, CLI, and OT networks. |
| **[Yubico (YubiKey as a Service)](https://www.yubico.com/)** | **~$1.0B Market Cap** (~$200M annual revenue, Nasdaq Stockholm: YUBICO) | **~$3.00–$4.00/user/month** (YubiEnterprise Subscription; Base/Advanced/Compliance tiers, 500-user minimum) | **No free tier**: physical hardware security keys subscription; offers sales-managed enterprise pilots with up to 25% annual replacement allowance | Hardware security keys with FIDO2/WebAuthn and PIV; YubiKey as a Service provides automated global key logistics and replacement pools across 190+ countries. |
| **[HYPR](https://www.hypr.com/)** | **~$200M Valuation** ($120M+ total venture funding raised) | **$3.00/user/month** (Identity Assurance Access); $6.00/user/month (Plus); $9.00/user/month (Advanced) | **30-day free trial**: evaluation pilot capped at up to 50 users for web and workstation passwordless access | True passwordless MFA platform utilizing FIDO2/WebAuthn, mobile biometrics, and desktop login verification. |
| **[Trusona](https://trusona.com/)** | **~$80M Valuation** ($38M total funding raised) | **Custom quote-based** (starting enterprise packages scale by Monthly Active Users / volume) | **Free tier available**: 100% free passwordless MFA plugin for WordPress; enterprise cloud offers sales-guided evaluation pilots (no time-limited self-serve trial) | Passwordless authentication leveraging mobile biometrics, dynamic identity proofing, and anti-ATO (account takeover) protection. |

## Open-Source GitHub Projects



- **[Authelia](https://github.com/authelia/authelia)**  

  **Single Sign-On Multi-Factor portal for web apps** (Apache-2.0) . **The lightweight option for protecting reverse proxy endpoints**—sits in front of Nginx, Traefik, or HAProxy and handles authentication and 2FA for services behind those proxies . **OpenID Certified™** for Basic OP, Implicit OP, Hybrid OP, Form Post OP, and Config OP profiles . **Features**: **OpenID Connect 1.0 / OAuth 2.0**, **FIDO2 WebAuthn security keys** (YubiKey), **TOTP**, **Duo mobile push**, **passwordless authentication via WebAuthn (Passkeys)**, **fine-grained access control** with rules matching subdomain/user/group/URI/method/network, **per-rule one-factor or two-factor policies**, **basic authentication support**, **high availability** with remote database and Redis, **Traefik ForwardAuth middleware** compatibility, **Caddy forward_auth directive** compatibility, and **Kubernetes Ingress Controller and Gateway support** . **Not a standalone directory**—does not replace OpenLDAP user management . **Best for**: teams whose primary requirement is protecting reverse proxy endpoints with minimal overhead .



- **[Keycloak](https://github.com/keycloak/keycloak)**  

  **Open Source Identity and Access Management** (Apache-2.0) . **The enterprise-grade choice**—handles **OIDC, SAML, and LDAP federation** natively with a fully customizable **account management console** covering password self-service . **Features**: **Single Sign-On** (authenticate once, access all apps; logout once, logged out of all), **Identity Brokering and Social Login** (add social networks through admin console—no code changes), **User Federation** (built-in LDAP and Active Directory support, custom providers for other stores), **Admin Console** (centrally manage features, identity brokering, user federation, applications, authorization policies, users, sessions), **Account Management Console** (update profile, change passwords, setup 2FA, manage sessions, link accounts), **Standard Protocols** (OpenID Connect, OAuth 2.0, SAML), and **Authorization Services** (fine-grained permissions from admin console) . **Integrates out of the box** with GitLab, Grafana, Nextcloud, and Sentry . **Trade-off**: operational complexity—heavyweight system to deploy and maintain with large configuration surface area . **Best for**: teams needing the full feature set with capacity to run it well .



- **[Authentik](https://github.com/goauthentik/authentik)**  

  **Open source Identity Provider that unifies your identity needs into a single platform** (MIT) . **The popular alternative to Keycloak**—significantly more approachable with modern UI and more intuitive configuration . **2025.4 release** adds **password history policy**, **Initial Permissions** for pre-defining object-level permissions on creation, **reputation score limits** with configurable numerical cap, **"remember me" option**, **PostgreSQL connection pools**, **Kubernetes Gateway API support (Preview)**, **LDAP group membership lookups based on user attributes** (including nested Active Directory groups), and **Provider Sync Dry Run** for SCIM/Google Workspace/Microsoft Entra providers . **"Forward Auth" capability** makes protecting Nginx-backed services with a unified login portal particularly straightforward . **Best for**: teams with mixed technical backgrounds or who want something maintainable without deep identity expertise .



- **[Casdoor](https://github.com/casdoor/casdoor)**  

  **UI-first Identity and Access Management (IAM) / Single-Sign-On (SSO) platform** (Apache-2.0) . **One place to manage users, organizations, applications, and providers** with a modern web console. **Authorization policies expressed with Casbin** (ACL, RBAC, ABAC, and more). **Unlike reverse-proxy-centric auth companions**, Casdoor is a **dedicated auth server with broad protocol support** . **Features**: **OAuth 2.0/OIDC**, **SAML 2.0**, **CAS**, **LDAP**, **WebAuthn/Passkeys**, **TOTP/MFA**, **Face ID**, **SCIM 2.0**, **RBAC**, **Social Login** (Google, GitHub, Azure AD), **Custom providers**, **User management web UI**, **Audit logs**, **Multi-tenancy**, **MCP Gateway**, **A2A Protocol**, **AI-First Design** . **Deploy via source, Docker all-in-one, Docker Compose, or Kubernetes Helm** . **Best for**: teams wanting a dedicated auth server with broad protocol support and AI/MCP integration.



- **[Ory](https://github.com/ory)**  

  **Modern, cloud-native authentication and authorization platform built for Kubernetes** (Apache-2.0) . **API-first design and headless architecture** (bring your own UI). **Components**: **Ory Hydra** (OAuth 2.0 and OpenID Connect server), **Ory Kratos** (Identity management), **Ory Oathkeeper** (Identity & Access Proxy), **Ory Keto** (Authorization server—Zanzibar-style) . **Requirements**: Go 1.21+, PostgreSQL/CockroachDB (production), Kubernetes recommended . **Best for**: cloud-native applications, microservices, Kubernetes-first deployments .



- **[SuperTokens](https://github.com/supertokens/supertokens-core)**  

  **Open-source alternative to Auth0** with simple integration (MIT) . **Developer-friendly APIs and embedded authentication** for modern frameworks. **Features**: **session management** (access/refresh tokens), **social login** (Google, GitHub), **email/password authentication**, **passwordless** (magic links, OTP), **pre-built UI components**, **self-hosted or managed cloud** . **Requirements**: Node.js 16+ or Python 3.7+ . **Best for**: developer-friendly APIs, embedded authentication, modern frameworks .



- **[Hanzo IAM](https://github.com/hanzoai/iam)**  

  **An open-source AI-first Identity and Access Management (IAM) / AI MCP gateway and auth server** (Apache-2.0) . **UI-first centralized authentication / Single-Sign-On (SSO) platform**. **Features**: **OAuth 2.0/OIDC provider**, **SAML/CAS/LDAP**, **WebAuthn/Passkeys**, **TOTP/MFA**, **Social login (40+ identity providers)**, **RBAC**, **Multi-tenancy**, **API-first**, **SCIM provisioning**, **RADIUS** . **Deploy via Docker, Docker Compose, or source** . **Best for**: AI-first organizations needing MCP/A2A protocol support.



- **[Perun](https://github.com/CESNET/Perun)**  

  **Identity and Access Management system covering management of the whole user life cycle** (FreeBSD licence) . **Developed by CESNET and Masaryk University in Brno, Czech Republic**. **Key features**: **virtual organisation management**, **user and group management**, **resource management**, **service management**, **identity consolidation (account linking)**, **push mechanism for authorisation data delivery**, **provisioning/de-provisioning of user rights on services**, **enrolment management** (customisable application forms), **delegation support**, **security teams support** (global user banning), **import and synchronisation** with existing identity/group management systems, **different Levels of Assurance**, **flexible attribute release policies**, **persistent and unique user identifiers**, **browser & non-browser based federated access**, **social media identities**, **effective accounting**, **e-Government integration** . **Supported standards**: VOOT, SAML2 IdP and AA (via Shibboleth IdP), various authentication protocols (via Apache AuthN modules), LDAP . **Dependencies**: PostgreSQL or Oracle DB, Java container, Shibboleth SP and IdP, OpenLDAP, Apache . **Production deployments**: Czech e-Infrastructure (CESNET), Masaryk University, ELIXIR, EGI . **Best for**: higher education or research institutions requiring VO management and federated identity .



- **[Maintainerd Auth](https://github.com/maintainerd/maintainerd-auth)**  

  **An open-source, self-hostable identity and access platform** (Apache-2.0) . **Delivers IAM for applications, services, and APIs**—from authentication and federation to fine-grained authorization. **Features**: **Full OAuth 2.0 + OIDC** (authorization code PKCE, client credentials, device, token exchange, PAR, CIBA, dynamic client registration, DPoP), **JWT (RS256)** with multi-key JWKS and automatic key rotation, **MFA** (TOTP, WebAuthn/passkeys, SMS OTP, backup codes, step-up auth), **Federation** (OIDC upstream connectors: Google, Microsoft, Apple, GitHub, GitLab; JIT provisioning; identity linking; home-realm discovery), **Fine-grained access control** (RBAC with granular permissions, IAM services, APIs, permissions, policies, service-token policy bundles, service-to-service authorization), **Multi-tenant** (full tenant isolation, API keys, invite flows), **Session management** (refresh token rotation, family revocation, reuse detection, concurrent session limits), **Webhook delivery** (auth event notifications with HMAC-SHA256 signatures and replay protection), **Audit logging** (structured auth events with retention, per-tenant isolation, PII redaction), **Pluggable secret management** (env vars, AWS Secrets Manager, SSM, HashiCorp Vault, Azure Key Vault, GCP Secret Manager), **Pluggable email providers** (SMTP, SES, SendGrid, Postmark, Mailgun, Resend), **OpenTelemetry** (traces, metrics, Prometheus endpoint) . **Quick start**: clone, configure `.env`, `docker compose up --build -d` . **Best for**: teams needing a modern, self-hostable IAM with comprehensive protocol support.



- **[Shibboleth](https://www.shibboleth.net/)**  

  **Web-based single sign-on (SSO) and federated identity solutions** for higher education and research institutions . **Expands user authentication systems** to grant access to online resources from associated organizations and promote seamless inter-organizational collaboration. **Features**: **embedded discovery service**, **federated identity management**, **centralized auditing and reporting** for user authentication events and application access, **user attributes exchange**, **single sign-on** . **Adheres to interoperability standards** and offers **community support** . **Pricing**: membership tiers based on IdP/SP counts (€12,500–€50,000 for NREN/Federation Members), users (€2,750–€8,250 for Academic/Non-Profit), or revenue (€5,500–€22,000 for Commercial) . **Best for**: higher education or research institutions requiring federated identity and resource sharing .



### Additional Strong Open-Source Options



- **[Ory Kratos](https://github.com/ory/kratos)** — Identity management component of Ory stack. **API-first, headless identity server** for cloud-native applications .

- **[Ory Hydra](https://github.com/ory/hydra)** — OAuth 2.0 and OpenID Connect server. **The most flexible OAuth2 server** for custom authorization flows .

- **[Ory Oathkeeper](https://github.com/ory/oathkeeper)** — Identity & Access Proxy. **Zero-trust networking** for microservices .

- **[Ory Keto](https://github.com/ory/keto)** — Authorization server implementing **Google Zanzibar-style** relationship-based access control .

- **[WSO2 Identity Server](https://github.com/wso2/product-is)** — Open-source IAM with SSO, MFA, and identity federation (Apache-2.0). **The most comprehensive enterprise-grade open-source IAM**.

- **[Gluu](https://github.com/GluuFederation/oxAuth)** — Open-source IAM platform with SSO, MFA, and federation (Apache-2.0). **The most flexible open-source IAM** for custom deployments.

- **[Casdoor (Chinese fork)](https://github.com/xiaoruiguo/casdoor)** — See Casdoor above .

- Community **n8n** workflows for authentication event routing and identity lifecycle automation.



**Frameworks for building custom systems**: Combine **Keycloak** for enterprise-grade IAM with **Authelia** for lightweight reverse proxy protection, **Authentik** for approachable UI and policy flexibility, **Casdoor** for dedicated auth server with AI/MCP integration, and **Ory** for cloud-native microservices—creating a fully self-hosted, enterprise-grade authentication platform.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Authentication and SSO systems handling credentials and personal data must comply with **FIDO2/WebAuthn standards, OAuth 2.0/OIDC specifications, SAML 2.0, and data protection regulations** (GDPR, CCPA, etc.).

- **Open-source authentication is mature and production-ready.** Keycloak is the enterprise-grade choice with full OIDC/SAML/LDAP federation . Authentik is the approachable alternative with modern UI and policy flexibility . Authelia is the lightweight reverse proxy companion with OpenID certification . Casdoor is the dedicated auth server with AI/MCP integration . **These are genuine alternatives to commercial platforms.**

- **The right choice depends on your architecture, not feature checklists.** Authelia protects reverse proxy endpoints—it's not a standalone directory and doesn't replace LDAP user management . Keycloak is a full identity platform but heavyweight to operate . Authentik balances capability with approachability . **Pick based on operational capacity and actual requirements.**

- **Passwordless authentication is the emerging standard.** Authelia supports WebAuthn Passkeys . Yubico's hardware keys provide phishing-resistant MFA with FIDO2/WebAuthn . Beyond Identity and HYPR eliminate passwords entirely. **The industry is converging on FIDO2 as the phishing-resistant foundation.**

- **AI-native IAM is the new frontier.** Hanzo IAM and Casdoor add **MCP Gateway** and **A2A Protocol** support—authentication for AI agents and model context protocols . **This is the emerging requirement for agent-augmented architectures.**

- Self-hosted open-source solutions require proper security hardening, certificate management, and ongoing maintenance. **Identity infrastructure is the control plane for your security**—compromise here undermines everything else.



---



**Made for platform engineers, security teams, and developers building transparent authentication solutions.**  

Let's make Authentication & SSO more open, data-driven, and passwordless.
