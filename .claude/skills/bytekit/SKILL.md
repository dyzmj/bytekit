```markdown
# bytekit Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches the development patterns and conventions used in the `bytekit` Java codebase. You'll learn about file naming, import/export styles, commit message practices, and how to write and organize tests. While no specific workflows were detected, this guide provides a foundation for consistent development and collaboration within the repository.

## Coding Conventions

### File Naming
- **Convention:** PascalCase is used for file names.
- **Example:**  
  ```java
  public class ByteParser { ... }
  // File: ByteParser.java
  ```

### Import Style
- **Convention:** Relative imports are preferred.
- **Example:**  
  ```java
  import mypackage.utils.ByteUtils;
  ```

### Export Style
- **Convention:** Named exports are used (standard in Java via `public` classes).
- **Example:**  
  ```java
  public class ByteKit { ... }
  ```

### Commit Messages
- **Style:** Freeform, no strict prefixes.
- **Average Length:** 42 characters.
- **Example:**  
  ```
  Fix bug in byte array parsing logic
  ```

## Workflows

_No explicit workflows detected in the repository. Below are suggested general workflows for Java development in this codebase._

### Adding a New Feature
**Trigger:** When implementing a new feature.
**Command:** `/add-feature`

1. Create a new Java file using PascalCase for the class name.
2. Implement the feature, using relative imports for dependencies.
3. Export the class with a `public` modifier.
4. Write corresponding tests in a file matching `*.test.*`.
5. Commit changes with a clear, concise message.

### Fixing a Bug
**Trigger:** When resolving a bug.
**Command:** `/fix-bug`

1. Locate the relevant Java file(s).
2. Apply the fix, maintaining existing code style.
3. Update or add tests to cover the bug scenario.
4. Commit with a message describing the fix.

## Testing Patterns

- **Framework:** Not explicitly detected.
- **File Pattern:** Test files follow the `*.test.*` naming convention.
- **Example:**  
  ```
  ByteParser.test.java
  ```
- **Practice:** Place test files alongside or within the test directory, and ensure they cover both typical and edge cases.

## Commands
| Command      | Purpose                                |
|--------------|----------------------------------------|
| /add-feature | Start workflow for adding a new feature|
| /fix-bug     | Start workflow for fixing a bug        |
```
