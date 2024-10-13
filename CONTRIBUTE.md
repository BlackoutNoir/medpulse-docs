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
