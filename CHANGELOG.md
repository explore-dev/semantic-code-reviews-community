# Changelog
All changes to semantic code reviews will be documented in this file.

## [0.4] - 2020-06-03

### Features

- Comments (Add/Remove/Edit)
- Submit pull request review
- Chat with us in the extension
- More support for TypeScript 3.9
- Back-end optimisations
- [**beta**] Pull request summary for GitHub app 

### API changes
#### Added
- `pr/check`: Get request used to check if back-end should analyse file changes
- `pr/comments`: Get request to retrieve comments
- `pr/comment/delete`: Post request to delete comment
- `pr/comment/edit`: Post request to edit comment
- `pr/comment/post`: Post request to post comment
- `pr/info`: Get request for basic information about pull request
- `pr/summary`: **[beta]** Get request for pull request summary of semantic changes
- `repo/delete`: Post request to remove repositories
- `org/delete`: Post request to remove organizations

#### Deprecated
- `pr/commits`: Superseded by `pr/info`.

## [0.3] - 2020-05-20
### Features

- Bidirectional code expansion
- Better syntax highlighting 

**No API changes**

## [0.2] - 2020-05-12
### Features

- Bidirectional code expansion
- Better syntax highlighting 

**No API changes**

## [0.1] - 2020-05-04
### Features

- Support for TypeScript
- Support for private repositories
- Code expansion

### API changes
#### Added
- `auth/start`: Get request to start authentication
- `auth/access`: Get request to finalize authentication
- `pr/code/context`: Post request to expand code around a symbol
- `pr/code/symbol`: Post request to expand code inside a symbol
- `pr/symbols`: Get request to retrieve symbols in pull request
- `repo/sync`: Post request to synchronise repository
- `repo/sync/status`: Get request to get status of repository
