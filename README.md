# Hello world javascript action

This action calculates a version based on the base version passed in.  
baseversion.buildnumber
if not off 'master' then it will be baseversion.buildnumber-branch

## Inputs

## `release-branch`

Name of the release branch - defaults to `"master"`.
## `base-version`

Base version of the product, like 6.0

## Outputs

## `version`

The version that was calculated.

## Example usage

```yaml
- name: calculate version
  uses: waynebrantley/github-branchversion@v1
  with:
    release-branch: 'main'
    base-version: '6.0'
```
