# Agent Instructions

This repository consumes the Sylphx engineering doctrine from [SylphxAI/doctrine](https://github.com/SylphxAI/doctrine).

Before changing files here:

- Read [PROJECT.md](./PROJECT.md) and [`.doctrine/project.json`](./.doctrine/project.json) for this repository's goal, lifecycle, boundary, public surfaces, and adoption gaps.
- Read `SylphxAI/doctrine` `AGENTS.md`, `PRINCIPLES.md`, and `ADR.md`, then load any triggered standards.
- Treat the Atoma API as a shared package contract; product-specific state models belong in consuming repositories.

Do not add application-specific state behavior here. This repository owns the Atoma core package only.
