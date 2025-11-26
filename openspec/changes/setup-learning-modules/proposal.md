# Change: Setup Learning Modules

## Why
The project currently lacks structure for organizing computer science learning materials. A structured module system for the 9 core Teach Yourself Computer Science subjects will enable clear learning paths, organized resource storage, and systematic progress through the curriculum.

## What Changes
- Create module structure for 9 subjects (Programming, Computer Architecture, Algorithms and Data Structures, Mathematics for CS, Operating Systems, Computer Networking, Databases, Languages and Compilers, Distributed Systems)
- Establish centralized resource directories for books, videos, and exercises
- Define module metadata format (prerequisites, programming languages, resource references)
- Provide module template for consistent structure

## Impact
- Affected specs: New capabilities `learning-module` and `resource-management`
- Affected code: New directories `modules/` and `resources/`, updated project README

## Summary
Organize learning materials for the 9 subjects from Teach Yourself Computer Science into a structured module system. Each module includes prerequisites, programming language requirements, resource organization (books, videos, exercises), and metadata for learning guidance.

## Motivation
The project currently lacks structure for organizing computer science learning materials. Creating a modular system for the 9 core subjects enables:

- Clear learning paths with prerequisites
- Organized storage for books, videos, and exercises
- Personal customization while maintaining professional structure
- Incremental content addition following minimal design principles

## Scope
This proposal covers:

1. **Learning Module Structure** - Define organization for 9 subjects with consistent metadata
2. **Resource Management** - Create directory structure for books, videos, and exercise materials
3. **Module Metadata** - Specify prerequisites, programming languages, and resource references

Out of scope:
- Actual learning content (added incrementally by user)
- Progress tracking implementation (future enhancement)
- Interactive exercises or automated testing

## User Impact
Provides a professional, minimal framework for organizing computer science learning materials with clear structure for future content addition.

## Alternatives Considered

### Alternative 1: Flat Directory Structure
Store all materials in subject-specific folders without metadata.

**Rejected because:** Lacks prerequisite tracking, language requirements, and scalability for cross-subject dependencies.

### Alternative 2: Database-Driven System
Use a database to manage learning materials and progress.

**Rejected because:** Over-engineered for initial needs; violates Occam's Razor principle; adds unnecessary complexity.

### Alternative 3: Git Submodules for Resources
Use git submodules to link external resources.

**Rejected because:** Complicates resource management; user owns book files directly; adds git complexity.

## Dependencies
None. This is the foundational structure for the learning project.

## Risks
- Risk: Inconsistent module structure if conventions aren't clear
  - Mitigation: Define explicit requirements and templates in specs

## Spec Deltas
1. `learning-module` - Core structure and conventions for subject modules
2. `resource-management` - Organization of books, videos, and exercises

## Implementation Notes
- Use Markdown for module metadata (readable, version-controllable)
- Keep structure minimal - extensible for future needs
- Follow conventions from project CLAUDE.md (professional tone, Occam's Razor)
