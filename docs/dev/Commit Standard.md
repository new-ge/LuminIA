# Commit Standard

## Simplified Standard for Commit Messages

Standardizing commit messages is an important practice. In addition to helping with the understanding of the change history, it also makes it easier to create automated tools based on the specification.

> This standard is a simplified version of [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).

---

### Message Format
```<Branch_id> - <type>: <description of the delivery made in the commit>```

- `<Branch_id>`: Identifier of the task in the task management system: Jira
- `<type>`: Type of change
- `<description of the delivery made in the commit>`: Clear description of what is being delivered

---

### Commit Types

| Type        | Description                                                              | Example                                                                 |
|-------------|--------------------------------------------------------------------------|-------------------------------------------------------------------------|
| `feat`      | When adding a new feature                                                | `LMN-1243 - feat: Implementation of repositories used for operations with climate variation tables` |
| `fix`       | Bug fix                                                                  | `LMN-56 - fix: Fix municipality selection component`                       |
| `docs`      | Documentation update                                                     | `LMN-5 - docs: Added database model diagram to the application`           |
| `style`     | Code style change (formatting), does not affect functionality            | `LMN-22 - style (AB-1243, AB-56): adjusted variable names to camelCase pattern`  |
| `refactor`  | Refactoring code, without changing functionality                         | `LMN-82 - refactor: improved structure of average calculation function`  |
| `test`      | Adding or modifying tests                                                | `LMN-79 - test: created unit tests for login component`                  |
| `chore`     | Minor updates that don’t directly impact functionality                   | `LMN-69 - chore: project dependency updates`                              |

---

### Fields Explained

- **`<Branch_id>`**: Identifier of the task created in the team’s task management tool, e.g., Jira.

- **`<description of the delivery made in the commit>`**: A clear description of what is being delivered in the commit created and pushed to Git.