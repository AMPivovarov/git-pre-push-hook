git-pre-push-hook
=================

git pre-push client-side hook, that prevents occasional errors with "--force" option.

## Sample config:

prevents deletion/corruption of tags and branches, except the "amp/feature" ones

```
[hooks]
  pushforceprotectedremotes = "origin"
  pushforceprotectedbranches = "(refs/tags/.*|refs/heads/(?!amp/.*).*)"
```

