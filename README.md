# sdist-release

This is simple script which creates source distribution from clean git
checkout. This avoids any problems with any uncommitted changes in working copy
and ensures that tag is pushed to the repository.

At the moment only github repositories are supported. 

# Installation

Program use only python standard library and expects that `wget` and `unzip` are
installed. Information about repositories is read from
`~/.config/sdist-release`:

```
[statistics]
github = haskell/statistics

[vector]
github = haskell/vector
subdir = vector
```

Use:

```
$ sdist-release package-name tag/commit_hash
```
