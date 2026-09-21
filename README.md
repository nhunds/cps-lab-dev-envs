# CPS Lab Dev Environments

This repository manages the containerized development environments for the Laboratory for Cyber-Physical Systems (CPS Lab).

## Goal
The primary objective is to provide a standardized, highly compatible development stack based on **ROS 2 Humble**. To ensure seamless access to GUI applications regardless of the host OS or environment, all graphical output is routed via **VNC** and **noVNC**.

## Project Structure
- **Base Image**: A robust ROS 2 Humble base image containing the core toolchain and VNC/noVNC infrastructure.
- **Devcontainer Features**: Modular extensions built on top of the base image to support specific development platforms (e.g., Niryo Ned 2).
- **Distribution**: Both the base image and the features are published to the **GitHub Container Registry (GHCR)**.

## Architecture
- **Base Stack**: Ubuntu $\rightarrow$ ROS 2 Humble $\rightarrow$ VNC Server $\rightarrow$ noVNC.
- **Modularization**: Use of Devcontainer Features allows platform-specific dependencies to be added without bloating the base image.

## Getting Started
*(Detailed setup instructions will be added as the implementation progresses)*

## Documentation
Design decisions are documented as Architecture Decision Records (ADRs) in the `docs/adrs` directory.
