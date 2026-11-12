# Mammoth Backend API

A backend REST API that serves fascinating facts about woolly mammoths, backed by Quarkus and PostgreSQL.

[![Contribute](https://img.shields.io/badge/Dev%20Spaces-Contribute-blue?logo=redhat&logoColor=white)](https://devspaces.apps.cluster-zc4gd.dyn.redhatworkshops.io/#https://github.com/shirodkar/mammoth-backend/tree/refactor)

## API

```
GET /mammoths/overview             — Mammoth overview
GET /mammoths/facts                — All mammoth facts
GET /mammoths/facts/{category}     — Facts by category
GET /mammoths/categories           — All categories
```
