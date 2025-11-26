# Spec: Resource Management

## Overview
Defines centralized organization for learning resources (books, videos, exercises) shared across modules. Resources are stored separately from module definitions to support flexible reuse and personal library management.

## ADDED Requirements

### Requirement: Resource Directory Structure
Learning resources MUST be organized in a centralized, subject-based hierarchy.

#### Scenario: Organizing textbook files
**Given** book resources for the learning project
**When** storing books
**Then** books are placed in `resources/books/<subject>/`
**And** subject names match module directory names
**And** subdirectories exist for all 9 core subjects:
  - programming
  - computer-architecture
  - algorithms-and-data-structures
  - mathematics-for-cs
  - operating-systems
  - computer-networking
  - databases
  - languages-and-compilers
  - distributed-systems

#### Scenario: Empty resource directories
**Given** a newly created resource directory
**When** the directory contains no files yet
**Then** a `.gitkeep` file preserves the directory in version control
**And** users can add resources incrementally

#### Scenario: Organizing video links
**Given** video lecture references for a subject
**When** storing video information
**Then** videos are documented in `resources/videos/<subject>/README.md`
**And** each entry includes: title, instructor, platform, URL, description
**And** videos are organized by course or lecture series

#### Scenario: Organizing exercise files
**Given** practice exercises for a subject
**When** storing exercise materials
**Then** exercises are placed in `resources/exercises/<subject>/`
**And** exercises are grouped by topic or difficulty
**And** each exercise includes problem statement and optional solutions

### Requirement: Resource Metadata
Resources MUST include sufficient metadata for discovery and selection.

#### Scenario: Book metadata
**Given** a textbook in the resources directory
**When** documenting the book in module README
**Then** metadata includes: title, author(s), edition, ISBN (optional)
**And** optional notes describe content coverage or recommended chapters
**And** optional difficulty assessment (beginner/intermediate/advanced)
**Example:**
```markdown
- **Computer Systems: A Programmer's Perspective** by Randal Bryant and David O'Hallaron (3rd Edition)
  - Practical programmer-oriented approach to computer architecture
  - Recommended: Chapters 1-6 for foundational understanding
  - Level: Intermediate
```

#### Scenario: Video lecture metadata
**Given** a video lecture series
**When** documenting videos in resources directory
**Then** metadata includes: course name, instructor, institution, platform, URL
**And** optional notes describe teaching style or content focus
**And** relationship to textbooks is noted if applicable
**Example:**
```markdown
### Berkeley CS 61A - Structure and Interpretation of Computer Programs
- **Instructor:** Brian Harvey
- **Platform:** archive.org
- **URL:** [Course archive](https://archive.org/details/ucberkeley-webcast-PL3E89002AA9B9879E)
- **Description:** Refined presentation of SICP concepts with better targeting for new students compared to MIT lectures
- **Pairs with:** Structure and Interpretation of Computer Programs textbook
```

#### Scenario: Exercise metadata
**Given** practice exercises in resources directory
**When** documenting exercises
**Then** metadata includes: topic, difficulty, estimated time, source (if external)
**And** exercises reference relevant sections in textbooks or lectures
**Example:**
```markdown
## Recursion Exercises
- **Source:** SICP Chapter 1
- **Difficulty:** Beginner to Intermediate
- **Estimated time:** 5-10 hours
- **Topics:** Recursive processes, tree recursion, iterative processes
```

### Requirement: Flexible Resource Organization
Resource organization MUST support incremental addition and personal customization.

#### Scenario: Adding books progressively
**Given** a resource directory for a subject
**When** adding new books over time
**Then** no predefined file structure is required
**And** any naming convention is acceptable
**And** books can be organized in subdirectories if desired
**And** module README is updated to reference new resources

#### Scenario: External resource links
**Given** resources available online
**When** documenting external resources
**Then** resources can be referenced by URL without local storage
**And** URL stability is noted if resource may become unavailable
**And** backup sources are listed if available
**Example:** Archive.org links for freely available course videos

#### Scenario: Mixed resource types
**Given** a subject with multiple resource types
**When** organizing materials
**Then** resources can span books, videos, exercises, and external links
**And** no resource type is mandatory for a valid module
**And** modules adapt based on available materials
**Example:** A module might start with only video links and add books later

### Requirement: Resource Discovery
Resources MUST be easily discoverable from module documentation and project root.

#### Scenario: Navigating from module to resources
**Given** a user reading a module README
**When** seeking recommended resources
**Then** relative links point to `../../resources/<type>/<subject>/`
**And** links work correctly from module directory location
**And** dead links are avoided by validating paths

#### Scenario: Browsing resources directory
**Given** a user exploring the resources directory
**When** examining available materials
**Then** directory structure clearly indicates subject areas
**And** README files in video directories provide resource descriptions
**And** exercise directories contain problem files and solutions

#### Scenario: Resource index in project root
**Given** a user starting from project README
**When** seeking overview of available resources
**Then** README links to both modules and resources directory
**And** summary indicates resource types available for each subject
**And** navigation paths are clear for both learning paths and resource browsing

## Dependencies
None.

## Cross-References
- `learning-module` - Defines module structure that references these resources
