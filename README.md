## Việc cần làm
**1️⃣ Cloud Platform Setup (GCP Free Tier)** 
 
- Create a **GCP project**  and enable billing.
 
- Set up **IAM roles**  for team members.
 
- Enable required **GCP services**  (Compute Engine, Kubernetes, Cloud SQL, etc.).
 
- Configure **budget alerts**  to prevent unexpected charges.

**2️⃣ Containerization & Deployment** 
 
- **Dockerize ERPNext**  and push to **Google Container Registry (GCR)** .
 
- Create a **GKE Autopilot cluster** .
 
- Write **Kubernetes deployment YAML**  for ERPNext.
 
- Deploy ERPNext **as a pod**  in GKE.

**3️⃣ Authentication (SSO)** 
 
- Set up **Auth0**  for authentication.
 
- Configure **OAuth2, SAML, JWT**  authentication.
 
- Integrate Auth0 with **ERPNext login** .
 
- Store **SSO credentials securely**  in Secret Manager.

**4️⃣ API Management** 
 
- Deploy **Kong API Gateway**  as a Kubernetes service.
 
- Configure **rate limiting**  and **authentication**  rules.
 
- Secure **API endpoints**  used by ERPNext.
 
- Route API traffic through **Kong** .

**5️⃣ CI/CD Automation** 
 
- Set up **GitHub Actions**  to automate builds and deployments.
 
- Write **CI/CD scripts**  for ERPNext container builds.
 
- Automate Kubernetes deployment using **GitHub Actions** .
 
- Monitor and debug pipeline execution.

**6️⃣ Database Setup** 
 
- Deploy **Google Cloud SQL (PostgreSQL Free Tier)** .
 
- Configure **database connections**  for ERPNext.
 
- Set up **automatic backups**  for the database.
 
- Optimize **database performance settings** .

**7️⃣ Caching & Session Management** 
 
- Deploy **Google Cloud Memorystore (Redis Free Tier)** .
 
- Configure ERPNext to use Redis for **session storage** .
 
- Optimize **Redis caching strategies** .
 
- Monitor **Redis performance** .

**8️⃣ Logging & Monitoring** 
 
- Enable **Google Cloud Operations Suite (Stackdriver)** .
 
- Configure **log collection**  for ERPNext & API Gateway.
 
- Set up **alerts**  for errors, crashes, and performance issues.
 
- Create **dashboards for monitoring**  Kubernetes & database.

**9️⃣ Secrets Management** 
 
- Store **SSO credentials, API keys, and DB passwords**  in **Google Secret Manager** .
 
- Configure **ERPNext & API Gateway**  to access secrets.
 
- Set up **automatic secret rotation policies** .

**🔟 Backup & Disaster Recovery** 
 
- Configure **Persistent Volume Snapshots**  for database backups.
 
- Automate **daily and weekly backup schedules** .
 
- Document **backup recovery process** .

**1️⃣1️⃣ Load Balancing & Auto-Scaling** 
 
- Deploy **Google Cloud Load Balancer** .
 
- Configure **ingress rules**  for ERPNext and API services.
 
- Set up **Horizontal Pod Autoscaler (HPA)**  to scale pods.
 
- Test **auto-scaling**  based on CPU usage.

| Task | Bach (Infrastructure) | Vy Anh (Application & API) | Sieu thi (DevOps & Security) | 
| --- | --- | --- | --- | 
| 1. Cloud Platform Setup (GCP, IAM, Billing) | ✅ |  |  | 
| 2. Containerization & Deployment (Docker, GKE) | ✅ |  |  | 
| 3. Authentication (SSO - Auth0 Integration) |  | ✅ |  | 
| 4. API Management (Kong Gateway, API Security) |  | ✅ |  | 
| 5. CI/CD Automation (GitHub Actions, Deployment Pipelines) |  |  | ✅ | 
| 6. Database (Cloud SQL PostgreSQL) | ✅ |  |  | 
| 7. Caching & Session Management (Redis) |  | ✅ |  | 
| 8. Logging & Monitoring (Stackdriver, Alerts, Dashboards) |  |  | ✅ | 
| 9. Secrets Management (Google Secret Manager) |  | ✅ |  | 
| 10. Backup & Disaster Recovery (Persistent Volume Snapshots, Restore Plans) |  |  | ✅ | 
| 11. Load Balancing & Auto-Scaling (GCP Load Balancer, HPA) |  |  | ✅ | 

<div align="center">
    <a href="https://erpnext.com">
        <img src="https://raw.githubusercontent.com/frappe/erpnext/develop/erpnext/public/images/erpnext-logo.png" height="128">
    </a>
    <h2>ERPNext</h2>
    <p align="center">
        <p>ERP made simple</p>
    </p>

[![CI](https://github.com/frappe/erpnext/actions/workflows/server-tests.yml/badge.svg?branch=develop)](https://github.com/frappe/erpnext/actions/workflows/server-tests.yml)
[![UI](https://github.com/erpnext/erpnext_ui_tests/actions/workflows/ui-tests.yml/badge.svg?branch=develop&event=schedule)](https://github.com/erpnext/erpnext_ui_tests/actions/workflows/ui-tests.yml)
[![Open Source Helpers](https://www.codetriage.com/frappe/erpnext/badges/users.svg)](https://www.codetriage.com/frappe/erpnext)
[![codecov](https://codecov.io/gh/frappe/erpnext/branch/develop/graph/badge.svg?token=0TwvyUg3I5)](https://codecov.io/gh/frappe/erpnext)
[![docker pulls](https://img.shields.io/docker/pulls/frappe/erpnext-worker.svg)](https://hub.docker.com/r/frappe/erpnext-worker)

[https://erpnext.com](https://erpnext.com)

</div>

ERPNext as a monolith includes the following areas for managing businesses:

1. [Accounting](https://erpnext.com/open-source-accounting)
1. [Warehouse Management](https://erpnext.com/distribution/warehouse-management-system)
1. [CRM](https://erpnext.com/open-source-crm)
1. [Sales](https://erpnext.com/open-source-sales-purchase)
1. [Purchase](https://erpnext.com/open-source-sales-purchase)
1. [HRMS](https://erpnext.com/open-source-hrms)
1. [Project Management](https://erpnext.com/open-source-projects)
1. [Support](https://erpnext.com/open-source-help-desk-software)
1. [Asset Management](https://erpnext.com/open-source-asset-management-software)
1. [Quality Management](https://erpnext.com/docs/user/manual/en/quality-management)
1. [Manufacturing](https://erpnext.com/open-source-manufacturing-erp-software)
1. [Website Management](https://erpnext.com/open-source-website-builder-software)
1. [Customize ERPNext](https://erpnext.com/docs/user/manual/en/customize-erpnext)
1. [And More](https://erpnext.com/docs/user/manual/en/)

ERPNext is built on the [Frappe Framework](https://github.com/frappe/frappe), a full-stack web app framework built with Python & JavaScript.

## Installation

<div align="center" style="max-height: 40px;">
    <a href="https://frappecloud.com/erpnext/signup">
        <img src=".github/try-on-f-cloud-button.svg" height="40">
    </a>
    <a href="https://labs.play-with-docker.com/?stack=https://raw.githubusercontent.com/frappe/frappe_docker/main/pwd.yml">
      <img src="https://raw.githubusercontent.com/play-with-docker/stacks/master/assets/images/button.png" alt="Try in PWD" height="37"/>
    </a>
</div>

> Login for the PWD site: (username: Administrator, password: admin)

### Containerized Installation

Use docker to deploy ERPNext in production or for development of [Frappe](https://github.com/frappe/frappe) apps. See https://github.com/frappe/frappe_docker for more details.

### Manual Install

The Easy Way: our install script for bench will install all dependencies (e.g. MariaDB). See https://github.com/frappe/bench for more details.

New passwords will be created for the ERPNext "Administrator" user, the MariaDB root user, and the frappe user (the script displays the passwords and saves them to ~/frappe_passwords.txt).


## Learning and community

1. [Frappe School](https://school.frappe.io) - Learn Frappe Framework and ERPNext from the various courses by the maintainers or from the community.
2. [Official documentation](https://docs.erpnext.com/) - Extensive documentation for ERPNext.
3. [Discussion Forum](https://discuss.erpnext.com/) - Engage with community of ERPNext users and service providers.
4. [Telegram Group](https://erpnext_public.t.me) - Get instant help from huge community of users.


## Contributing

1. [Issue Guidelines](https://github.com/frappe/erpnext/wiki/Issue-Guidelines)
1. [Report Security Vulnerabilities](https://erpnext.com/security)
1. [Pull Request Requirements](https://github.com/frappe/erpnext/wiki/Contribution-Guidelines)
1. [Translations](https://translate.erpnext.com)


## License

GNU/General Public License (see [license.txt](license.txt))

The ERPNext code is licensed as GNU General Public License (v3) and the Documentation is licensed as Creative Commons (CC-BY-SA-3.0) and the copyright is owned by Frappe Technologies Pvt Ltd (Frappe) and Contributors.

By contributing to ERPNext, you agree that your contributions will be licensed under its GNU General Public License (v3).

## Logo and Trademark Policy

Please read our [Logo and Trademark Policy](TRADEMARK_POLICY.md).
