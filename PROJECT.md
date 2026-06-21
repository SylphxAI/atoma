# SylphxAI Atoma

SylphxAI/atoma is a TypeScript state-management library experiment centered on a framework-agnostic `atom()` and `store()` API.

## Lifecycle

- State: `incubating`
- Layer: `foundation`
- Machine manifest: [`.doctrine/project.json`](./.doctrine/project.json)

## Goals

- Provide a minimal framework-agnostic state management core with atoms, stores, computed state, async state, streams, models, and families.
- Keep the public package surface focused on `src/index.ts`, `src/atom.ts`, `src/store.ts`, and `src/types.ts`.
- Stabilize the family API and TypeScript inference before production lifecycle promotion.

## Non-Goals

- This repository does not own application-specific state models or UI framework integrations until they are explicitly added.
- This repository does not own downstream product behavior that consumes the package.
- This repository does not own enterprise engineering doctrine.

## Boundary

This repository owns the Atoma core package, package docs, tests, and release workflow. UI framework adapters, product-specific state models, and consuming application behavior belong in their own repositories unless promoted through a documented shared package contract.

## Public Surfaces

- Package README: [`README.md`](./README.md)
- Package manifest and scripts: [`package.json`](./package.json)
- Public export entry: [`src/index.ts`](./src/index.ts)
- Atom implementation: [`src/atom.ts`](./src/atom.ts)
- Store implementation: [`src/store.ts`](./src/store.ts)
- Public types: [`src/types.ts`](./src/types.ts)
- Test suite: [`src/store.spec.ts`](./src/store.spec.ts)
- Release workflow: [`.github/workflows/release.yml`](./.github/workflows/release.yml)

## Delivery

The repository has a main-branch release workflow that delegates to the central SylphxAI/.github reusable release workflow, but repo memory records current TypeScript errors from an incomplete family API refactor. Production proof requires `npm run build`, `npm test`, typecheck once added/enforced, and release workflow or package-registry readback. This manifest slice is documentation-only and does not change package code, tests, release behavior, or package metadata.
