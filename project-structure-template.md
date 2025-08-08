# Standard Data Engineering Project Structure

```
project-name/
├── README.md                   # Project overview and setup
├── .env.example                # Environment variables template
├── .gitignore                  # Git ignore patterns
├── requirements.txt            # Python dependencies (or package.json for Node)
├── docker-compose.yml          # Local development environment
├── Dockerfile                  # Container build instructions
│
├── src/                        # Source code
│   ├── __init__.py
│   ├── config.py              # Configuration management
│   ├── main.py                # Application entry point
│   ├── models/                # Data models and schemas
│   │   ├── __init__.py
│   │   └── schemas.py
│   ├── services/              # Business logic
│   │   ├── __init__.py
│   │   ├── processor.py
│   │   └── publisher.py
│   └── utils/                 # Utility functions
│       ├── __init__.py
│       ├── logging.py
│       └── retry.py
│
├── tests/                     # Test files
│   ├── __init__.py
│   ├── conftest.py           # Pytest configuration
│   ├── unit/                 # Unit tests
│   │   ├── test_processor.py
│   │   └── test_publisher.py
│   ├── integration/          # Integration tests
│   │   └── test_e2e.py
│   └── fixtures/             # Test data
│       └── sample_data.json
│
├── scripts/                  # Deployment and utility scripts
│   ├── deploy.sh
│   ├── setup.sh
│   └── run_tests.sh
│
├── infrastructure/           # Infrastructure as Code
│   ├── terraform/           # Terraform configurations
│   │   ├── main.tf
│   │   └── variables.tf
│   └── k8s/                # Kubernetes manifests
│       └── deployment.yaml
│
├── docs/                    # Additional documentation
│   ├── architecture.md
│   ├── deployment.md
│   └── troubleshooting.md
│
└── tasks/                   # Project management
    └── todo.md             # Task tracking (as per workflow protocol)
```

## Key Conventions
- **src/**: All application source code
- **tests/**: Mirror src/ structure for easy navigation
- **scripts/**: Executable scripts for common operations
- **infrastructure/**: IaC and deployment configurations
- **docs/**: Detailed documentation beyond README
- **planning/**: Project planning and task tracking