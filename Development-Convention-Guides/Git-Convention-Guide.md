## Repository name
- Use hyphen as separators (e.g. mac-base)

## Branch name
- Use slash and hyphen as separators (e.g. feature/add-documentation)
- Avoid long descriptive names

## Git submodule URL
- Use the form: `https://dev.azure.com/thordrive/{ProjectName}/_git/{RepositoryName}`
- Do not include `{UserName}@` in submodule URL.

  >**Bad**👎
  >```cmd
  >https://thordrive@dev.azure.com/thordrive/revolt/_git/dev-convetion
  >```

  >**Good**👍
  >```cmd
  >https://dev.azure.com/thordrive/revolt/_git/dev-convetion
  >```