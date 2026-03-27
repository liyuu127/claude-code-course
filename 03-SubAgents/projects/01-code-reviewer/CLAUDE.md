# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Purpose

This is a **teaching demo** for configuring a `code-reviewer` subagent with minimal read-only permissions. The source files in `src/` intentionally contain security vulnerabilities for review demonstration purposes.

## Code Reviewer Agent

A `code-reviewer` agent is configured in `.claude/agents/code-reviewer.md`:


### Usage

```
让 code-reviewer 审查 src/auth.js 的安全性
让 code-reviewer 检查最近提交的代码质量
让 code-reviewer 看一下我刚改的代码
```

## Intentional Vulnerabilities (Do Not Fix)

| File | Issue Types |
|------|-------------|
| `src/auth.js` | Hardcoded secrets, weak encryption, eval usage, password in response |
| `src/database.js` | SQL injection, hardcoded credentials, sensitive logging |
| `src/api.js` | No rate limiting, CORS misconfiguration, path traversal, debug endpoint |

These vulnerabilities are intentional for demonstrating the reviewer's detection capabilities.