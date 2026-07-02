```markdown
# english Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches the core development patterns and conventions used in the `english` TypeScript codebase. It covers file naming, import/export styles, commit message structure, and testing patterns. While no frameworks or automated workflows are detected, this guide will help you write consistent, maintainable code and collaborate effectively within this repository.

## Coding Conventions

### File Naming
- **Style:** kebab-case
- **Example:**  
  ```plaintext
  my-component.ts
  string-utils.test.ts
  ```

### Import Style
- **Style:** Relative imports
- **Example:**  
  ```typescript
  import { myFunction } from './utils';
  ```

### Export Style
- **Style:** Named exports
- **Example:**  
  ```typescript
  // In utils.ts
  export function myFunction() { /* ... */ }
  
  // In another file
  import { myFunction } from './utils';
  ```

### Commit Messages
- **Style:** Conventional commits
- **Prefix:** `feat`
- **Average Length:** ~27 characters
- **Example:**  
  ```
  feat: add string capitalization utility
  ```

## Workflows

_No automated workflows detected in this repository._

## Testing Patterns

- **Framework:** Unknown (no explicit framework detected)
- **File Pattern:** `*.test.*`
- **Example:**  
  ```typescript
  // string-utils.test.ts
  import { capitalize } from './string-utils';

  describe('capitalize', () => {
    it('capitalizes the first letter', () => {
      expect(capitalize('hello')).toBe('Hello');
    });
  });
  ```
- **How to Run:**  
  Use your preferred TypeScript test runner (e.g., Jest, Mocha) to execute files matching `*.test.*`.

## Commands
| Command        | Purpose                                             |
|----------------|-----------------------------------------------------|
| /conventions   | Show coding conventions and code style guidelines   |
| /test-patterns | Show how to write and run tests in this repository  |
```