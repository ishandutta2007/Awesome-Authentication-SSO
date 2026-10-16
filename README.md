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

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Duo Security (Cisco)](https://duo.com/)**  

  **The most widely adopted MFA platform** with push notifications, TOTP, WebAuthn, and SMS verification. Features **adaptive authentication**, **device trust**, and **zero-trust access policies**. **Integrated with Authelia** as a mobile push provider .



- **[Okta Verify](https://www.okta.com/)**  

  **Enterprise identity cloud** with SSO, MFA, lifecycle management, and API access management. Features **Universal Directory**, **Adaptive MFA**, and **Identity Governance**. **The enterprise standard** for workforce and customer identity.



- **[Microsoft Entra ID](https://www.microsoft.com/en-us/security/business/identity-access/microsoft-entra-id)**  

  **Microsoft's cloud identity platform** (formerly Azure AD) with SSO, Conditional Access, and passwordless authentication. Features **Entra Verified ID** for decentralized identity and **Entra Permissions Management** for CIEM.



- **[Ping Identity](https://www.pingidentity.com/)**  

  **Enterprise IAM platform** with SSO, MFA, API security, and identity governance. **Merged with ForgeRock** to combine AI-driven IAM with fraud and risk protection . **PingOne for Workforce** starts at $3/user/month for 5,000+ users .



- **[RSA SecurID](https://www.rsa.com/)**  

  **The original hardware token MFA**—now a comprehensive access management platform with **risk-based authentication**, **identity governance**, and **zero-trust capabilities**.



- **[Silverfort](https://www.silverfort.com/)**  

  **Unified identity protection platform** that extends MFA to any resource—including legacy systems, OT networks, and command-line interfaces—without agents or proxies.



- **[Beyond Identity](https://www.beyondidentity.com/)**  

  **Passwordless authentication** with **device-bound credentials** and **continuous risk assessment**. Eliminates passwords entirely while providing phishing-resistant MFA.



- **[HYPR](https://www.hypr.com/)**  

  **Passwordless authentication** with **FIDO2/WebAuthn** and **decentralized identity**. Features **HYPR Affirm** for identity verification and **HYPR Adapt** for risk-based authentication.



- **[Trusona](https://trusona.com/)**  

  **Passwordless authentication** using **mobile device biometrics** and **identity proofing**. Features **Trusona Authentication Cloud** for consumer-facing applications.



- **[Yubico Cloud (YubiKey as a Service)](https://www.yubico.com/)**  

  **Hardware security keys** with **FIDO2/WebAuthn** and **PIV** support. **YubiKey as a Service** expands to **199 delivery locations** (175 countries and 24 territories) with **self-service ordering** for employees in the US, Canada, and Europe . **The gold standard** for phishing-resistant hardware MFA.



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
