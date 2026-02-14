# 📡 SmartSuper API Documentation Portal

> **Role-based API console** — safe to share with vendors without exposing source code.

🔗 **Live URL:** [https://anand4286.github.io/smart-super-api-docs/](https://anand4286.github.io/smart-super-api-docs/)

---

## 🎭 Role-Based Views

| Role | What They See | Who Uses It |
|------|--------------|-------------|
| **🤝 External / Vendor** | Only `External`-tagged APIs (31 endpoints) | Super fund partners, ATO integrators, accountant platforms |
| **📱 UI / Mobile** | `External` + `UI`-tagged APIs (66 endpoints) | iOS developers, frontend team |
| **⚙️ Internal / Ops** | All APIs including `Internal` (86 endpoints) | Backend team, DevOps, compliance |
| **🌐 All** | Everything | Architecture review, full audit |

## 📊 API Coverage

| Service | Proto File | RPCs | External | UI | Internal |
|---------|-----------|------|----------|----|----------|
| UserService | `user/v1/user_service.proto` | 14 | 5 | 7 | 0 |
| SuperFundService | `super/v1/super_fund_service.proto` | 17 | 10 | 5 | 1 |
| TaxService | `tax/v1/tax_service.proto` | 10 | 5 | 3 | 1 |
| AIInsightsService | `ai/v1/ai_insights_service.proto` | 13 | 5 | 7 | 0 |
| DocumentService | `document/v1/document_service.proto` | 7 | 3 | 3 | 1 |
| NotificationService | `notification/v1/notification_service.proto` | 11 | 0 | 9 | 2 |
| ComplianceService | `compliance/v1/compliance_service.proto` | 12 | 2 | 1 | 9 |
| Health | `common/v1/common.proto` | 2 | 1 | 0 | 1 |
| **TOTAL** | | **86** | **31** | **35** | **15** |

## 🔐 What's Safe to Share

✅ **This portal contains NO:**
- Source code
- API keys or secrets
- Infrastructure details
- Database schemas
- Internal business logic

✅ **Only contains:**
- API endpoint paths
- HTTP methods
- gRPC RPC names
- Authentication requirements
- Scope/permission requirements
- Endpoint descriptions

## 🔄 Keeping in Sync

This portal is auto-generated from the Protocol Buffer definitions in `smart-super-api`. When proto files change:

1. Run `scripts/generate-api-docs.sh` in `smart-super-platform`
2. Copy updated `index.html` to this repo
3. Push to `main` — GitHub Pages auto-deploys

---

*Source: `smart-super-api/proto/smartsuper/` | © 2026 SmartSuper Pty Ltd*