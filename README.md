Markdown
# MCP Schema Guard 🛡️

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/VISHALSAI12/mcp-schema-guard/pulls)
[![MCP Protocol Version](https://img.shields.io/badge/MCP%20Spec-2024--11--05-blueviolet)](https://modelcontextprotocol.io)

A lightweight developer utility and pre-commit checker designed to validate, inspect, and benchmark **Model Context Protocol (MCP)** tool schemas and server definitions before deploying AI agents.

---

## 🎯 The Problem

When developing agentic workflows with Claude and other LLMs, tool schemas frequently suffer from subtle formatting errors:
- Missing required fields in JSON Schema declarations
- Ambiguous or non-string tool descriptions that trigger model hallucination
- Incompatible input property definitions that waste expensive API tokens at runtime

**MCP Schema Guard** catches these mismatches locally in your terminal or CI pipeline before runtime execution.

---

## ✨ Features

- **Schema Assertion:** Verifies input and output structures against the official Model Context Protocol specifications.
- **Ambiguity Linter:** Flags incomplete parameter definitions and tool descriptions prone to model misinterpretation.
- **Local Pre-Flight Checks:** Run dry-run validations without making external network or API calls.
- **CI/CD Ready:** Integrate directly into GitHub Actions or local git pre-commit hooks.

---

## 🚀 Quick Start

### Installation

Clone the repository and install dependencies locally:

```bash
git clone [https://github.com/VISHALSAI12/mcp-schema-guard.git](https://github.com/VISHALSAI12/mcp-schema-guard.git)
cd mcp-schema-guard
npm install
