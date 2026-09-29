# Lab Creation Guide

## Lab Structure

Each lab lives in `labs/<category>/<lab-name>/` with:

```
labs/web/sql-injection-basic/
├── Dockerfile          # Vulnerable app container
├── lab.yml             # Lab metadata
├── README.md           # Lab description shown to users
└── solution.md         # Solution (maintainers only)
```

## lab.yml Format

```yaml
name: "SQL Injection — Login Bypass"
category: web
difficulty: easy         # easy | medium | hard | expert
xp: 100
level_required: 1
flag: "flag{sql_inject10n_b4sics}"
tags: [sqli, owasp, authentication]
author: "Your Name"
description: "Bypass the login form using SQL injection"
hints:
  - cost: 25
    text: "What happens when you add a single quote to the username?"
  - cost: 50
    text: "Try: ' OR 1=1 --"
```

## Creating a New Lab

1. Pick a category and difficulty
2. Build a vulnerable Docker app
3. Create the `lab.yml` config
4. Write a clear `README.md` for users
5. Write `solution.md` with step-by-step walkthrough
6. Test locally with `docker build` and `docker run`
7. Submit a PR!
