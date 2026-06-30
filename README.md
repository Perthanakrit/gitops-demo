# gitops-demo

### Example Directory Structure

```
├── apps/
│   ├── guestbook/                      # Application 1
│   │   ├── base/
│   │   │   ├── deployment.yaml
│   │   │   ├── service.yaml
│   │   │   └── kustomization.yaml
│   │   └── environments/
│   │       ├── dev/
│   │       │   └── kustomization.yaml  # Dev-specific changes (e.g., 1 replica)
│   │       └── prod/
│   │           └── kustomization.yaml  # Prod-specific changes (e.g., 5 replicas)
│   │
│   └── todo-api/                       # Application 2
│       ├── base/
│       └── environments/
│           ├── dev/
│           └── prod/
│
└── bootstrap/                          # The "Application Set" root controller
    └── applicationset.yaml
```
