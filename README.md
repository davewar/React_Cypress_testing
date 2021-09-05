https://github.com/testing-library/cypress-testing-library/blob/main/README.md

# CYPRESS SET UP

A) install dev dependencies": { "@testing-library/cypress": "^7.0.6", "cypress":
"^7.4.0", "eslint-plugin-cypress": "^2.11.3"}

b) Add file named "jsconfig.json" for intelisense.

c) Access cy commands by adding

- import '@testing-library/cypress/add-commands' to cypress > support>
  commands.js

D) Add file named ".eslintrc.json" for eslint.

E) Add file named "cypress.json" with base url.

F) remove default fixtures and integration tests.

cypress> delete files in the fixtures and integration folders

G) add below to .gitignore file

```
/coverage
/cypress/videos
/cypress/screenshots

```

# Writing tests

add tests in cypress/integration. Files should be in the format of
"xxxxxxxxx_spec.js"

# CI/CD

add netlify.toml file - will run tests before build / deploy

# Branch Protection Rules

github> settings> branches > branch protection rules > add rule. branch name =
eg main

tick a) Require pull request reviews before merging b) Require conversation
resolution (people can comment on your code and every comment must be resolved
on github by the creator or the responder of the comment) > Create button.
