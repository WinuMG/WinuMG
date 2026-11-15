<div align="center">

# Winuka Mahagamage

<a href="https://github.com/WinuMG">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=3500&pause=800&color=2F81F7&center=true&vCenter=true&width=640&lines=Backend-focused+Software+Engineer;Java+%7C+Spring+Boot+%7C+Node.js+%7C+TypeScript;Distributed+Systems+%E2%80%A2+Identity+%E2%80%A2+DevOps;Building+an+OAuth+2.1+server+from+scratch" alt="Typing SVG" />
</a>

**Computer Science Undergraduate @ University of Colombo School of Computing (UCSC)**
<br/>
Software Engineering Intern candidate · Matara, Sri Lanka 🇱🇰

<p>
  <a href="https://linkedin.com/in/winuka-mahagamage"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:winukauni@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://github.com/WinuMG"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
  <img src="https://komarev.com/ghpvc/?username=WinuMG&style=for-the-badge&color=2F81F7&label=PROFILE+VIEWS" alt="Profile views"/>
</p>

</div>

---

### `$ whoami`

```java
public record Engineer(
        String name,
        String role,
        List<String> focus,
        List<String> architectures,
        String currentlyBuilding,
        String openTo
) {
    public static Engineer winuka() {
        return new Engineer(
            "Winuka Mahagamage",
            "CS Undergraduate @ UCSC · Freelance Web Developer",
            List.of("Backend Engineering", "Auth & Identity", "CI/CD & DevOps"),
            List.of("Microservices", "Modular Monolith", "Event-Driven / Saga", "REST"),
            "AgentPass — an OAuth 2.1 / OIDC identity server for AI agents",
            "Software Engineering Internships"
        );
    }
}
```

I build backend systems that hold up in production: services that talk over message brokers, auth layers that check every request, and pipelines that refuse to merge untested code. One of my systems is **live and in daily use at the Road Development Authority, Matara**.

---

### 🛠️ Tech Stack

<table>
  <tr>
    <td><b>Languages</b></td>
    <td><img src="https://skillicons.dev/icons?i=java,ts,js,python,php&theme=dark" alt="Languages"/></td>
  </tr>
  <tr>
    <td><b>Backend</b></td>
    <td><img src="https://skillicons.dev/icons?i=spring,nodejs,express,nestjs&theme=dark" alt="Backend"/></td>
  </tr>
  <tr>
    <td><b>Data</b></td>
    <td><img src="https://skillicons.dev/icons?i=postgres,mysql,mongodb,redis&theme=dark" alt="Databases"/></td>
  </tr>
  <tr>
    <td><b>Messaging</b></td>
    <td><img src="https://skillicons.dev/icons?i=rabbitmq&theme=dark" alt="Messaging"/>&nbsp;
        <img src="https://img.shields.io/badge/Socket.IO-010101?style=flat-square&logo=socketdotio&logoColor=white" alt="Socket.IO" height="28"/>
        <img src="https://img.shields.io/badge/WebSockets-4A4A55?style=flat-square" alt="WebSockets" height="28"/></td>
  </tr>
  <tr>
    <td><b>Frontend</b></td>
    <td><img src="https://skillicons.dev/icons?i=react,nextjs,vite,tailwind,html,css&theme=dark" alt="Frontend"/></td>
  </tr>
  <tr>
    <td><b>DevOps</b></td>
    <td><img src="https://skillicons.dev/icons?i=docker,kubernetes,githubactions,nginx,aws,linux&theme=dark" alt="DevOps"/></td>
  </tr>
  <tr>
    <td><b>Quality</b></td>
    <td>
      <img src="https://img.shields.io/badge/SonarQube-4E9BCD?style=flat-square&logo=sonarqube&logoColor=white" alt="SonarQube" height="28"/>
      <img src="https://img.shields.io/badge/SonarCloud-F3702A?style=flat-square&logo=sonarcloud&logoColor=white" alt="SonarCloud" height="28"/>
      <img src="https://img.shields.io/badge/JaCoCo-C21325?style=flat-square" alt="JaCoCo" height="28"/>
      <img src="https://img.shields.io/badge/Testcontainers-291A3F?style=flat-square&logo=testcontainers&logoColor=white" alt="Testcontainers" height="28"/>
      <img src="https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white" alt="Vitest" height="28"/>
      <img src="https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white" alt="Flyway" height="28"/>
    </td>
  </tr>
</table>

---

### 🚧 Currently Building: AgentPass

> **An identity server for AI agents, written from scratch.** AI agents increasingly act *on behalf of* users. AgentPass gives them access that is scoped, time-limited and fully audited, never the user's own credentials.

```mermaid
sequenceDiagram
    autonumber
    participant U as User
    participant A as AI Agent
    participant AP as AgentPass (OAuth 2.1 / OIDC)
    participant R as Resource API

    U->>AP: Authenticate (Passkey / WebAuthn)
    A->>AP: Token Exchange (RFC 8693) — act on behalf of user
    AP-->>U: Risky action? Approve via CIBA
    U-->>AP: Approved
    AP->>A: Delegated, scoped, short-lived token
    A->>R: Call API with delegated token
    R-->>AP: Every action audited
```

`Java 21` `Spring Boot` `PostgreSQL` `Redis` `React` `TypeScript` `Python` `Docker` `Kubernetes`

---

### 🏗️ Featured Engineering Work

<table>
<tr>
<td width="50%" valign="top">

#### 🚚 [SwiftTrack](https://github.com/WinuMG/swifttrack)
**Microservices Logistics Platform** · *Grade A*

- Independent **Node.js microservices** behind an **API gateway** with JWT auth
- **Saga orchestration** over **RabbitMQ** keeps distributed order transactions consistent
- **Protocol adapters** connect legacy systems
- Real-time delivery tracking pushed to the React dashboard with **Socket.IO**

`Node.js` `RabbitMQ` `MongoDB` `Docker Compose`

</td>
<td width="50%" valign="top">

#### 🌾 AgriTech Connect
**Farm Management & Agri-Trading Platform**

- **11-module modular monolith** with Spring Modulith
- Stateless **JWT** auth + role-based authorisation via **Spring Security**
- **PostgreSQL + PostGIS** schema, versioned migrations with **Flyway**
- CI/CD: **SonarQube** gates, **JaCoCo** coverage, **Testcontainers**, images published to **GHCR**

`Java 25` `Spring Boot 4` `Valkey` `GitHub Actions`

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### 💼 [TalentPipe](https://github.com/Multi-Tenant-Recruitment-Platform)
**Multi-Tenant SaaS Recruitment Platform** · *UCSC Industry Project*

- **Led the React + TypeScript frontend** in a 5-person Agile team, mentored by a Senior SWE
- JWT auth with **silent token refresh**, **RBAC for 4 roles**, **tenant data-isolation guard**
- Integrated with a **Spring Boot** REST API
- **Vitest** tests and CI through **Docker + GitHub Actions + SonarCloud**

[`frontend`](https://github.com/Multi-Tenant-Recruitment-Platform/talentpipe-frontend) · [`backend`](https://github.com/Multi-Tenant-Recruitment-Platform/talentpipe-backend)

</td>
<td width="50%" valign="top">

#### 🛣️ RDA Matara — Road Projects System
**🟢 Live in production at the Road Development Authority**

- Full-stack platform that monitors road projects run by private contractors and presents them to the public
- **JWT role-based workflows** for engineers, technical officers, supervisors and staff
- Real-time project tracking with **Google Maps API** visualisation
- Containerised with **Docker**, served behind **Nginx**

`React` `Express` `MongoDB` `Nginx`

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### 🍞 Toast Vibes POS
**Restaurant Point-of-Sale System**

- **NestJS** server-side billing with automated reporting and scheduled backups
- Live order and status sync on every dashboard via **WebSockets**
- JWT-secured, role-based dashboards

`NestJS` `TypeScript` `MongoDB` `shadcn/ui`

</td>
<td width="50%" valign="top">

#### ⚽ GoPlay
**Sports Booking & E-Commerce Platform** · *Grade A*

- Built on a **custom PHP MVC framework** with a MySQL relational schema
- **Led the Coach module**: time-slot validation, availability scheduling, earnings analytics, reviews
- PayHere payments, Chart.js analytics

`PHP` `MySQL` `Chart.js` `PayHere`

</td>
</tr>
</table>

---

### 🧠 Engineering Principles

```yaml
architecture:   Choose the simplest structure that scales: modular monolith first, microservices when needed
consistency:    Distributed transactions need sagas, not hope
security:       Deny by default · least privilege · validate every token
quality:        If CI doesn't check it, it isn't guaranteed: tests, coverage gates, static analysis
delivery:       Containerise everything · reproducible builds · migrations are code
```

---

### 📜 Certifications

| Certification | Issuer | Status |
|---|---|---|
| DevOps Fundamentals | IBM | ✅ Jun 2026 |
| API Development | Edureka · Coursera | ✅ Nov 2026 |
| Machine Learning Specialization | DeepLearning.AI & Stanford Online | 🔄 In progress |

---

### 📊 GitHub Activity

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=WinuMG&show_icons=true&hide_border=true&theme=github_dark&count_private=true" height="165" alt="GitHub stats"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=WinuMG&layout=compact&hide_border=true&theme=github_dark&langs_count=8" height="165" alt="Top languages"/>
  <br/>
  <img src="https://streak-stats.demolab.com?user=WinuMG&hide_border=true&theme=github-dark-blue" alt="GitHub streak"/>
  <br/>
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=WinuMG&theme=github-compact&hide_border=true&area=true" width="100%" alt="Contribution graph"/>
</div>

---

<div align="center">

**Open to Software Engineering Internships, especially backend, platform and DevOps roles.**

<a href="mailto:winukauni@gmail.com"><img src="https://img.shields.io/badge/Let's_talk-winukauni%40gmail.com-2F81F7?style=for-the-badge&logo=maildotru&logoColor=white" alt="Contact"/></a>

<sub>English · Sinhala</sub>

</div>
