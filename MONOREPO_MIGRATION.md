# Monorepo Migration

This package is being consolidated into the sathergate-toolkit Turborepo monorepo.

## What Changed
- tsconfig.json now extends a shared base config (../../tsconfig.base.json)
- Package will live under packages/{npm-name}/ in the monorepo
- Build orchestration moves to Turborepo (turbo run build)
- Shared devDependencies hoisted to monorepo root

## Monorepo Structure
packages/
  shutterbox/      (darkroom)
  flagpost/        (flagpost)
  ratelimit-next/  (floodgate)
  notifykit/       (herald)
  croncall/        (clocktower)
  vaultbox/        (lockbox)
  searchcraft/     (sifter)
