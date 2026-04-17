<div align="center">

# BOUACIDA LOUAI

```
╔═══════════════════════════════════════════════════════════╗
║  ROLE     ▸  Backend Java Developer                       ║
║  FOCUS    ▸  Microservices · Security · Distributed Sys   ║
║  STATUS   ▸  Building production-grade backends           ║
║  LOCATION ▸  Algeria 🇩🇿                                   ║
╚═══════════════════════════════════════════════════════════╝
```

[![GitHub followers](https://img.shields.io/github/followers/Bouacida-Louai?style=flat-square&color=6DB33F&labelColor=1a1a2e)](https://github.com/Bouacida-Louai)
[![Email](https://img.shields.io/badge/✉-abderrahmane.bouacida@univ--constantine2.dz-1a1a2e?style=flat-square)](mailto:abderrahmane.bouacida@univ-constantine2.dz)

</div>

---

```java
@Developer
public class BouacidaLouai {

    private final String role       = "Backend Java Developer";
    private final String[] passions = { "Security Engineering",
                                        "Distributed Systems",
                                        "Clean Architecture" };

    public Architecture design() {
        return new Microservices()
                   .with(SpringCloud.EUREKA, SpringCloud.GATEWAY)
                   .secured(Keycloak.v24, OAuth2.JWT)
                   .resilient(Resilience4j.CIRCUIT_BREAKER)
                   .containerized(Docker.COMPOSE)
                   .build();
    }
}
```

---

## ⚙️ Stack

<table>
<tr>
<td valign="top" width="33%">

**Core**
```
Java
Spring Boot 3
Spring Security 6
Spring Data JPA
```

</td>
<td valign="top" width="33%">

**Microservices**
```
Spring Cloud
Eureka · API Gateway
Feign Client
Resilience4j
```

</td>
<td valign="top" width="33%">

**Security**
```
Keycloak 24
OAuth2 · JWT
RBAC · BCrypt
Custom Permission Eval
```

</td>
</tr>
<tr>
<td valign="top">

**Database**
```
MySQL 8 · H2
JPA / Hibernate
Pessimistic Locking
ACID Transactions
```

</td>
<td valign="top">

**DevOps**
```
Docker · Docker Compose
Git · Postman
Swagger / OpenAPI
```

</td>
<td valign="top">

**Testing**
```
JUnit 5
Mockito
Unit & Integration Tests
```

</td>
</tr>
</table>

---

## 🗂️ Projects

### `01` — Microservices E-Commerce Platform

```
┌─────────────┐     ┌────────────────┐     ┌───────────────┐
│  API Gateway│────▶│  Config Server │     │ Eureka Server │
│  JWT Filter │     │  (Centralized) │     │ (Discovery)   │
└──────┬──────┘     └────────────────┘     └───────┬───────┘
       │                                           │
       ├──────────────────────────────────────────┤
       │                                           │
  ┌────▼──────┐  ┌─────────────┐  ┌──────────────▼───┐
  │ Product   │  │   Order     │  │   Inventory      │
  │ Service   │  │   Service   │  │   Service        │
  └───────────┘  └──────┬──────┘  └──────────────────┘
                        │  Feign + Circuit Breaker
                 ┌──────▼──────┐
                 │  Payment    │
                 │  Service    │
                 └─────────────┘
  [All 7 services · Docker Compose · Single-command deploy]
```

> `Spring Boot 3` `Spring Cloud` `JWT` `Resilience4j` `Docker Compose` `H2`

---

### `02` — SecureBank API

```
  USER REQUEST
       │
  ┌────▼──────────────────────────────────────────┐
  │           Keycloak 24 + OAuth2 + JWT           │
  │              6 Roles · Auto Realm Import        │
  └────┬──────────────────────────────────────────┘
       │
  ┌────▼────────────────────────────────────────────────┐
  │  Custom BankPermissionEvaluator + @PreAuthorize     │
  │  Amount-aware RBAC · Fine-grained Authorization     │
  └────┬────────────────────────────────────────────────┘
       │
  ┌────▼────────────────┐    ┌────────────────────────┐
  │  Transaction Engine │    │  Fraud Detection       │
  │  Pessimistic Lock   │    │  ① Large amount        │
  │  REPEATABLE_READ    │    │  ② High-frequency      │
  │  ACID Compliance    │    │  ③ Unusual-hour flag   │
  └─────────────────────┘    └────────────────────────┘
```

> `Spring Boot 3` `Spring Security 6` `Keycloak 24` `MySQL 8` `JPA/Hibernate` `Docker`

---

### `03` — Secure Auth & Authorization System

```
POST /auth/login
    │
    ├── BCrypt verification
    ├── Custom JWT generation
    └── Stateless response (no sessions)

GET /api/resource
    │
    ├── JWT Filter (custom)
    ├── GrantedAuthority evaluation
    │     ├── PERM_READ   → allowed
    │     ├── PERM_WRITE  → allowed
    │     └── PERM_DELETE → role-gated
    └── @RestControllerAdvice (global errors)

[JUnit 5 + Mockito coverage on all auth flows]
```

> `Spring Boot 3` `Spring Security` `JWT` `MySQL` `JPA/Hibernate` `BCrypt`

---

## 📋 Experience & Education

| Period | Role | Details |
|--------|------|---------|
| 2025 · 4 months | **Backend Developer Intern** @ NAFTAL | Spring Boot APIs · JWT security · Docker · Agile sprints |
| 2022 – 2024 | **B.Sc. Computer Science** · Univ. Constantine 2 | Information Systems · Final project: RBAC attendance tracker |

---

## 📊 GitHub Activity

<div align="center">

![Stats](https://github-readme-stats.vercel.app/api?username=Bouacida-Louai&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true)

![Streak](https://streak-stats.demolab.com?user=Bouacida-Louai&theme=tokyonight&hide_border=true)

</div>

---

<div align="center">

```
> Currently focused on: deeper Kubernetes patterns + reactive Spring
> Open to: backend roles, security-focused projects, remote work
> Reach me at: abderrahmane.bouacida@univ-constantine2.dz
```

*"Build it secure. Build it scalable. Build it right."*

</div>
