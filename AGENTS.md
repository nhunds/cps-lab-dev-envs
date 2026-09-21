# AGENTS.md - Instructions for Autonomous Agents

This document provides guidelines and context for autonomous AI agents (like `goose`) working on this repository to ensure consistency, maintainability, and adherence to lab standards.

## Core Principles
1. **Granular Commits**: Every change should be committed in small, logical increments. Use Conventional Commits (e.g., `feat:`, `fix:`, `docs:`, `refactor:`, `chore:`).
2. **Documentation First**: Before implementing significant changes, document the design decision as an Architecture Decision Record (ADR) in `docs/adrs`.
3. **Compatibility**: Priority is given to maximum compatibility. GUI applications must be accessible via VNC/noVNC.
4. **Modularity**: Prefer Devcontainer Features over monolithic images. The base image should remain lean.

## Workflow for Agents
- **Analyze First**: Use `tree` and `analyze` tools to understand the current state.
- **Plan**: Update the `todo` list before starting a task.
- **Implement**:
    - Create a feature-specific branch (e.g., `feat/feature-name`).
    - Write code/configs.
    - Verify changes.
- **Document**: If a design choice is made (e.g., choosing a specific VNC server), create an ADR.
- **Commit**: Use descriptive commit messages.

## Technical Context
- **Base OS**: Ubuntu (via ROS 2 Humble image).
- **Middleware**: ROS 2 Humble.
- **GUI Access**: VNC $\rightarrow$ noVNC (Web-based).
- **Packaging**: GHCR (GitHub Container Registry).
- **Configuration**: `.devcontainer` standards.

## ADR Format
When creating an ADR in `docs/adrs/ADR-XXX.md`, use the following structure:
- **Title**: Short name of the decision.
- **Status**: Proposed / Accepted / Superseded.
- **Context**: What is the problem? Why is a decision needed?
- **Decision**: What is the chosen solution?
- **Consequences**: What are the trade-offs? What improves? What becomes harder?
