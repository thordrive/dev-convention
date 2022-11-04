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

  >**Good**👝
  >```cmd
  >https://dev.azure.com/thordrive/revolt/_git/dev-convetion
  >```

## Large file storage
- Make sure install Git LFS on your system before cloning repositories.
- Track binary files or large output text files (e.g. Jupyter Notebook files - *.ipynb) with Git LFS.
