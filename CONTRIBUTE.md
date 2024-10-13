## Commit Message Guidelines

We use the **Conventional Commits** format to structure our commit messages. A good commit message helps to communicate the context of your change.

**Format:**
```JS
<type>(<scope>): <description>

[optional body]

[optional footer(s)]
```

### Commit Types:
* feat: A new feature
* fix: A bug fix
* docs: Documentation only changes
* style: Changes that do not affect the meaning of the code (white-space, formatting, etc.)
* refactor: A code change that neither fixes a bug nor adds a feature
* test: Adding or correcting tests
* chore: Changes to the build process or auxiliary tools and libraries

### Example Commit Message
```JS
feat(auth): add login functionality

Implemented user login using OAuth2. Added login form and user authentication logic.

BREAKING CHANGE: Updated login API to use OAuth2, existing tokens are no longer valid.
```

### Additional Guidelines:
* Use the imperative mood (e.g., "add feature", not "added feature").
* Separate subject from body with a blank line.
* Limit the subject line to 50 characters.
* Wrap the body at 72 characters.

### Branching Workflow
We follow the **Git Feature Branch Workflow**. Here's how to work with branches in this project:

- **Main Branch (`main`):** This is the production-ready branch. It contains stable code and should always be deployable.
- **Development Branch (`develop`):** This branch contains the latest work in progress. All new features, bug fixes, and improvements should be merged here first.
- **Feature Branches:** Each new feature should be developed in its own branch off develop. Name your feature branches descriptively (e.g., `feature/user-auth`, `bugfix/login-issue`).
- **Hotfix Branches:** For critical fixes that need to be applied to `main` immediately, create a branch named `hotfix/description`.

### Branch Naming Conventions
- **Features:** `feat/short-description`
- **Bug Fixes:** `fix/short-description`
- **Chore/Non-code tasks:** `chore/task-description`
- **Hotfixes:** `hotfix/issue-description`
