# Design: Setup Learning Modules

## Architectural Overview

This change establishes a dual-hierarchy structure for organizing computer science learning materials:

1. **Modules** (`modules/<subject>/`) - Subject-specific learning paths with metadata
2. **Resources** (`resources/<type>/<subject>/`) - Centralized storage for books, videos, exercises

This separation enables flexible resource reuse across modules while maintaining clear subject-based organization.

## Key Design Decisions

### Decision 1: Separate Modules and Resources

**Context:** Learning materials can be organized in a flat subject structure or with separation between learning paths and content storage.

**Decision:** Separate module metadata from resource storage.

**Rationale:**
- Modules focus on learning path (prerequisites, objectives, sequence)
- Resources focus on content storage (books, videos, exercises)
- Same resource can be referenced by multiple modules
- Resources can be added incrementally without restructuring modules
- Clear separation between "what to learn" and "materials for learning"

**Consequences:**
- Additional directory level introduces indirection
- Requires relative path links between modules and resources
- Clearer organization as project scales
- Easier to manage resources independently

### Decision 2: Subject-Based Resource Organization

**Context:** Resources could be organized by type (all books together) or by subject (subject-specific subdirectories).

**Decision:** Use `resources/<type>/<subject>/` hierarchy.

**Rationale:**
- Mirrors the 9-subject structure of Teach Yourself Computer Science
- Natural alignment with module organization
- Easier discovery of subject-specific materials
- Supports incremental addition per subject
- Scales well as subjects expand independently

**Consequences:**
- More directories initially (even if empty with .gitkeep)
- Clear correspondence between modules and resources
- Subject-focused browsing experience

### Decision 3: Markdown-Based Metadata

**Context:** Module metadata could use YAML frontmatter, JSON files, or Markdown documents.

**Decision:** Use Markdown README files with structured sections.

**Rationale:**
- Human-readable without special tools
- Version-controllable with meaningful diffs
- Renders nicely on GitHub and in editors
- Flexible formatting for descriptions and notes
- Familiar to developers
- Aligns with project preference for professional documentation

**Consequences:**
- No machine-parseable schema enforcement
- Relies on convention over validation
- Easy to write and maintain
- Natural reading experience

### Decision 4: Module Template Approach

**Context:** Modules could be generated programmatically or created from a copyable template.

**Decision:** Provide a template module that gets copied and customized.

**Rationale:**
- Simple, no tooling required
- Clear example of expected structure
- Easy to customize per subject
- Demonstrates conventions through example
- Follows minimal complexity principle

**Consequences:**
- Manual copying required for each module
- Consistency depends on following template
- Low barrier to entry
- Flexibility to deviate when needed

### Decision 5: Flexible Resource Addition

**Context:** Resource directories could enforce specific file structures or allow flexible organization.

**Decision:** Support flexible, user-controlled resource organization.

**Rationale:**
- Books are user-owned files with varying naming conventions
- Video links stored in README (no file structure needed)
- Exercises vary widely in format and organization
- Occam's Razor: don't impose structure where it's not needed
- Supports personal customization preference

**Consequences:**
- No enforced file naming conventions
- Module READMEs must explicitly reference resources
- Users maintain their own organization within subject directories
- Lower initial structure, higher flexibility

## Data Flow

1. **Module Discovery:** User starts at project README → navigates to specific module
2. **Learning Path:** User reads module README → understands prerequisites and objectives
3. **Resource Access:** User follows links from module → accesses books, videos, or exercises
4. **Direct Browsing:** User can also browse resources directory directly by subject

## Scalability Considerations

### Adding Subjects
New subjects can be added beyond the initial 9 by:
1. Creating new module directory
2. Adding corresponding resource subdirectories
3. Updating project README

### Resource Growth
As resources expand:
- Subdirectories within subject folders organize by topic
- Multiple video series can coexist with clear documentation
- Exercise sets can grow without restructuring

### Cross-Subject Resources
Resources relevant to multiple subjects:
- Store in most relevant subject directory
- Reference from multiple modules with relative links
- Optionally create `resources/cross-subject/` if needed

## Alternative Architectures Considered

### Flat Structure
All modules and resources in single directories.
**Rejected:** Poor scalability, cluttered navigation, no clear organization.

### Monolithic Subject Directories
Each subject contains both metadata and resources in one directory.
**Rejected:** Tight coupling, difficult resource reuse, complex directory structure.

### Database-Driven
Store metadata in SQLite or JSON database.
**Rejected:** Over-engineered, requires tooling, violates simplicity principle, poor version control experience.

### Git Submodules
External resources as submodules.
**Rejected:** Complexity overhead, user owns book files directly, unnecessary git abstraction.

## Technology Stack

- **Markdown:** Documentation and metadata
- **Git:** Version control
- **File System:** Resource storage
- **OpenSpec:** Change management and specification

## Testing Strategy

- Manual validation of directory structure
- Link validation (modules → resources)
- OpenSpec validation for spec compliance
- Review for professional documentation standards
- Verification of 9 subject coverage

## Future Considerations

### Potential Enhancements (Out of Scope)
- Progress tracking (completion checkmarks, notes)
- Automated link validation
- Resource search functionality
- Spaced repetition reminders
- Community resource contributions

These enhancements can be proposed as separate OpenSpec changes after foundational structure is established.

## Success Criteria

1. All 9 subjects have module directories with consistent structure
2. Resource directories exist for books, videos, and exercises
3. Module template demonstrates clear conventions
4. Project README provides navigation to all modules
5. Professional documentation quality throughout
6. OpenSpec validation passes with zero errors
7. Structure supports incremental resource addition
