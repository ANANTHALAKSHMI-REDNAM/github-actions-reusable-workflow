# github-actions-reusable-workflow

Git Basics
    ✓ Branching
    ✓ Merge
    ✓ Pull / Push

GitHub Actions
    ✓ Workflow triggers
    ✓ Jobs
    ✓ Steps
    ✓ Actions marketplace

Python CI
    ✓ Lint
    ✓ Tests

Optimization
    ✓ Cache

Build Management
    ✓ Artifacts

Containerization
    ✓ Docker build
    ✓ Docker run

Container Registry
    ✓ GHCR push
    ✓ GHCR versioning

Release Management
    ✓ Git tags
    ✓ Automatic versioning

Deployment
    ✓ DEV environment
    ✓ PROD environment
    ✓ Approval gate

Reusable Workflows
    ✓ workflow_call
    ✓ Inputs
    ✓ Secrets
    ✓ Multiple consumer repositories

Environment Management
    ✓ Variables
    ✓ Secrets
    ✓ Approvals











                    v1.2.0
                       │
                       ▼
              Reusable Workflow
                       │
             ┌─────────┴─────────┐
             ▼                   ▼
           Lint                Test
             │                   │
             └─────────┬─────────┘
                       ▼
                 Docker Build
                       │
                       ▼
                  Docker Run
                       │
                       ▼
                 Push to GHCR
                       │
                 :v1.2.0
                       │
                       ▼
                  DEV Deploy
                       │
                       ▼
              PROD Approval ⏸
                       │
                   Approved
                       │
                       ▼
                  PROD Deploy