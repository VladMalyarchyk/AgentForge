# PROJECT SPECIFICATION

## Project Purpose
AgentForge is a lightweight AI agent workspace that enables users to describe tasks in natural language and have AI agents plan, execute, and validate tasks using controlled tools.

## Portfolio Goals
- Demonstrate AI agent orchestration
- Showcase LLM tool calling and structured outputs
- Provide a clear, interview-ready architecture
- Demonstrate full-stack integration (React + FastAPI)
- Include security and validation boundaries
- Show real-world tool execution

## Core Functionality
- Task description parsing
- Agent planning and execution
- Tool registry and validation
- Result artifact generation

## MVP Scope
- Single-agent task execution
- Basic tool system (web_search, extract_text, etc.)
- Simple result validation
- No authentication or microservices

## Technology Stack
- Frontend: React + TypeScript + Vite + Tailwind CSS
- Backend: FastAPI + Python + Pydantic + SQLAlchemy
- Database: PostgreSQL
- LLM: Provider-agnostic abstraction (OpenAI/Ollama/Mock)

## Agent Architecture
```
User
  ↓
Task
  ↓
Planner
  ↓
Structured Plan
  ↓
Executor
  ↓
Tool Registry
  ↓
Tools
  ↓
Validator
  ↓
Result / Artifact
```

## Tool System
- Explicit tool registration
- Input validation
- URL validation
- Execution timeouts
- Max iteration limits

## Security Boundaries
- No unrestricted shell/Python/filesystem/network access
- Provider-specific security boundaries
- Input sanitization

## Data Model
- Task records
- Execution logs
- Tool metadata
- Result artifacts

## Explicit Non-Goals
- No microservices architecture
- No authentication system
- No complex task chaining
- No real-time execution
- No external API integrations (except for LLM providers)

## LLM Provider Abstraction
- OpenAI
- Ollama
- Mock provider for testing
- Provider-specific configuration management

## API Responsibilities
- Task management
- Agent execution
- Tool registration
- Result retrieval

## Frontend Responsibilities
- Task description input
- Execution progress tracking
- Result visualization
- CSV export

## Database Responsibilities
- Task storage
- Execution logging
- Tool metadata
- Result artifacts

## Testing Requirements
- Unit tests for core components
- Integration tests for agent execution
- Security testing for input validation

## Deployment Requirements
- Docker support
- CI/CD pipeline
- Local LLM support

## Portfolio Demo Requirements
- Simple task execution workflow
- Clear documentation
- Minimal dependencies
- No unnecessary complexity

## Future Roadmap
- Advanced tool system
- Multi-agent orchestration
- Real-time execution
- Security hardening
- Testing framework
- Docker/CI polish

