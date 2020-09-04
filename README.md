# About

This repository contains resume(s)/CVs of its creator organized in manageable and maintainable way.

## Contents

* `config/` - supporting configuration, package imports, style, macros, etc.
* `test/` - various tests for non-trivial custom commands and packages
* `resumes/` - actual resumes bodies
* `resumes/lowlevel/` - focus on low-level skills (C/C++ and related stuff)
* `resumes/java/` - focus on Java and web development
* `main.tex` - trick to simplify relative path management, root document for the `subfiles` package
* `sensitive.tex` - file, nonexistent by default, where sensitive information (home address, phone, etc.) may be provided

## Building

Just as simple as it looks:

```bash
cd resumes/lowlevel/
latexmk -pdf resume-en.tex
```

See CI/CD config for more elaborate build configuration.

## CI/CD

GutHub Actions and GitLab Runner are both supported. Release/artifact management is only configured for the former and only in its primitive form (no release versioning).
