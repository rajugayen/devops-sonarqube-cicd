# Automated CI/CD with GitHub Actions + SonarQube + Docker + AWS
Developer
   │
   │ git push
   ▼
┌─────────────────┐
│     GitHub      │
│   Repository    │
└────────┬────────┘
         │
         │ GitHub Actions
         ▼
┌─────────────────┐
│  CI/CD Pipeline │
├─────────────────┤
│ Checkout        │
│ Build/Test      │
│ SonarQube Scan  │
│ Quality Gate    │
└────────┬────────┘
         │
      PASS
         │
         ▼
┌─────────────────┐
│ Docker Build    │
│ Docker Push     │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│      AWS        │
│   Deployment    │
└─────────────────┘
