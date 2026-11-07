# Mammoth Backend API

A Java EE 8 backend REST API that serves fascinating facts about woolly mammoths, backed by JPA and PostgreSQL.

[![Contribute](https://img.shields.io/badge/Dev%20Spaces-Contribute-blue?logo=redhat&logoColor=white)](https://devspaces.apps.cluster-zc4gd.dyn.redhatworkshops.io/#https://github.com/shirodkar/mammoth-backend)

## Architecture

| Layer | Technology |
|-------|-----------|
| Runtime | JBoss EAP 8 |
| API | JAX-RS 2.1 |
| Persistence | JPA 2.2 / Hibernate |
| Database | PostgreSQL 15 |
| Build | Maven |
| Java | 17 |

## Getting Started

### Prerequisites

- Java 17
- Maven 3.8+
- PostgreSQL 15 (or use Dev Spaces — see badge above)

### Build

```bash
mvn clean install
```

### Run Tests

```bash
mvn clean verify
```

## Project Structure

```
mammoth-backend/
├── src/main/java/com/example/mammoth/
│   ├── api/          — JAX-RS resource and application
│   ├── model/        — JPA entity (MammothFact)
│   └── service/      — Business logic (MammothFactService)
├── src/test/java/    — Unit and integration tests
├── init-db.sql       — Database seed script
├── devfile.yaml      — OpenShift Dev Spaces configuration
└── pom.xml           — Project POM
```

## API

```
GET /backend/api/mammoths          — All mammoth facts
GET /backend/api/mammoths/{id}     — Single fact by ID
GET /backend/api/mammoths/random   — Random fact
```
