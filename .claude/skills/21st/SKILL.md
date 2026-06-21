```markdown
# 21st Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill provides a comprehensive guide to the coding conventions and workflows used in the "21st" TypeScript codebase, built with Next.js. It covers file naming, import/export styles, commit message patterns, and testing practices to ensure consistency and maintainability across the project.

## Coding Conventions

### File Naming
- Use **camelCase** for all file names.
  - Example: `userProfile.ts`, `orderHistory.test.ts`

### Import Style
- Use **relative imports** for referencing modules within the project.
  - Example:
    ```typescript
    import { fetchData } from './apiUtils';
    ```

### Export Style
- Use **named exports** for functions, components, and constants.
  - Example:
    ```typescript
    // apiUtils.ts
    export function fetchData() { ... }
    export const API_URL = '...';
    ```

### Commit Messages
- Follow the **conventional commit** format.
- Use the `build` prefix for build-related changes.
- Keep commit messages concise (average length: 76 characters).
  - Example:
    ```
    build: update Next.js to v13.4 and fix deployment script
    ```

## Workflows

*No automated workflows were detected in this repository. You may consider adding workflows for build, test, or deployment automation.*

## Testing Patterns

- **Test File Pattern:** All test files follow the `*.test.*` naming convention.
  - Example: `userProfile.test.ts`
- **Testing Framework:** Not explicitly detected. Use the standard test runner for TypeScript/Next.js projects (e.g., Jest or Vitest).
- **Test Example:**
  ```typescript
  // userProfile.test.ts
  import { getUserProfile } from './userProfile';

  describe('getUserProfile', () => {
    it('returns user data for a valid ID', () => {
      // test implementation
    });
  });
  ```

## Commands

| Command      | Purpose                                   |
|--------------|-------------------------------------------|
| /conventions | Show coding conventions and examples       |
| /test        | Run all tests in the project              |
| /build       | Build the Next.js application             |
| /commit      | Show commit message guidelines            |
```
