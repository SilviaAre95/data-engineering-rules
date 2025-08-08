# 🏗️ Claude Data Engineering Codex

*Transform your data engineering workflow from chaotic to systematic*

**Claude Data Engineering Codex** is your blueprint for building bulletproof, production-ready GCP data pipelines with AI assistance. No more ad-hoc solutions, scattered best practices, or reinventing the wheel—just consistent, scalable, and maintainable data engineering that grows with your needs.

> *"From simple Beam pipelines to complex multi-service architectures, build it right the first time."*

## Overview

This repository provides:
- **Workflow protocols** for systematic development with AI assistants
- **Data engineering best practices** specifically for GCP environments  
- **Adaptive project structures** that scale from simple pipelines to complex systems
- **Clean code principles** for maintainable, testable data engineering solutions

## Repository Structure

```
data-engineering-rules/
├── README.md                          # This file
├── CLAUDE.md                          # General workflow protocol (always active)
├── data-engineering-rules.md          # Data engineering specific rules
├── project-structure-template.md      # Adaptive project structures
```

## How It Works

### 1. General Workflow Protocol (`CLAUDE.md`)
Always active rules that Claude follows for any project:
- **Define the problem**: Clarify requirements and ask questions
- **Think & scan first**: Analyze codebase before making changes
- **Plan with todos**: Create actionable checklists in `planning/todo.md`
- **Check-in gate**: Get approval before implementing
- **Execute iteratively**: Small steps with progress updates
- **Prefer simplicity**: Minimal changes, avoid over-engineering

### 2. Data Engineering Rules (`data-engineering-rules.md`)
Specialized rules for data engineering projects:
- **Production-ready code**: Security, observability, idempotency
- **GCP best practices**: Cloud Run, Dataflow, Pub/Sub, BigQuery
- **Clean code principles**: SOLID, DRY, meaningful names
- **Testing strategies**: Unit tests, integration tests, Beam testing
- **Project organization**: References adaptive structure guidelines

### 3. Adaptive Project Structure (`project-structure-template.md`)
Three complexity levels that grow with your project:

**Basic** (< 500 lines): Simple Beam pipeline, single Cloud Function
```
project/
├── main.py
├── config.py  
├── test_main.py
└── planning/todo.md
```

**Intermediate** (500-2000 lines): Multiple components, shared utilities
```
project/
├── src/
│   ├── main.py
│   ├── transforms/
│   └── utils/
├── tests/
└── planning/todo.md
```

**Advanced** (2000+ lines): Multiple services, infrastructure, extensive testing
```
project/
├── src/
│   ├── pipeline/
│   ├── api/
│   └── shared/
├── tests/
├── infrastructure/
└── planning/todo.md
```

## Getting Started

### Option 1: Use with Claude Code (Recommended)

1. **Place rules in your project root:**
   ```bash
   git clone https://github.com/yourusername/data-engineering-rules.git
   cd your-data-project/
   cp ../data-engineering-rules/CLAUDE.md .
   cp ../data-engineering-rules/data-engineering-rules.md .
   ```

2. **Claude will automatically:**
   - Follow the workflow protocol in `CLAUDE.md`
   - Apply data engineering rules from `data-engineering-rules.md`
   - Create appropriate project structure based on complexity
   - Generate `planning/todo.md` for task tracking

3. **Start any request with:**
   ```
   "Help me build a Beam pipeline that processes user events"
   ```
   Claude will define the problem, scan existing code, create a plan, and ask for approval before coding.

### Option 2: Use with Cursor IDE

#### Setup Instructions

1. **Copy rules to your project:**
   ```bash
   cp CLAUDE.md your-project/.cursor-rules
   cat data-engineering-rules.md >> your-project/.cursor-rules
   ```

2. **Create Cursor Rules file:**
   ```bash
   # In your project root
   echo "# Data Engineering Rules for Cursor" > .cursor-rules
   echo "" >> .cursor-rules
   cat CLAUDE.md >> .cursor-rules
   echo "" >> .cursor-rules
   echo "---" >> .cursor-rules
   echo "" >> .cursor-rules
   cat data-engineering-rules.md >> .cursor-rules
   ```

3. **Configure Cursor:**
   - Open your project in Cursor
   - The `.cursor-rules` file will be automatically detected
   - Start any chat with: "Follow the data engineering rules and help me..."

#### Cursor-Specific Adaptations

- **File watching**: Cursor will automatically apply rules to new files
- **Code completion**: Rules influence autocomplete suggestions  
- **Refactoring**: Right-click → "Refactor with rules" applies data engineering principles
- **Project structure**: Cursor will suggest appropriate structure based on complexity

#### Workflow with Cursor

1. **Create planning directory:**
   ```bash
   mkdir planning
   touch planning/todo.md
   ```

2. **Start any request:**
   ```
   @cursor Follow the workflow protocol and help me create a Pub/Sub to BigQuery pipeline
   ```

3. **Cursor will:**
   - Define the problem and ask clarifying questions
   - Scan your codebase for existing patterns
   - Create a plan in `planning/todo.md`
   - Ask for approval before implementing
   - Execute iteratively with progress updates

## Key Benefits

- **Consistent quality**: All projects follow the same high standards
- **Scalable structure**: Grows appropriately with project complexity  
- **Production ready**: Built-in security, monitoring, and reliability patterns
- **Team collaboration**: Standardized workflow and conventions
- **Reduced errors**: Systematic approach with built-in reviews

## Examples

### Simple Beam Pipeline (Basic Structure)
Claude will create:
- `main.py` with Beam pipeline
- `config.py` with typed configuration
- `test_main.py` with DoFn unit tests
- `planning/todo.md` tracking implementation

### Multi-Service System (Advanced Structure)
Claude will create:
- Separate services in `src/pipeline/` and `src/api/`
- Shared utilities in `src/shared/`
- Comprehensive test suite in `tests/`
- Infrastructure code in `infrastructure/`

## Contributing

1. Fork this repository
2. Make your changes following the workflow protocol
3. Create `planning/todo.md` with your implementation plan
4. Submit PR with clear description of changes

## License

MIT License - Feel free to adapt for your organization's needs.

## Support

- Review the workflow protocol in `CLAUDE.md`
- Check data engineering rules in `data-engineering-rules.md`  
- Reference project structures in `project-structure-template.md`
- Open GitHub issues for questions or improvements