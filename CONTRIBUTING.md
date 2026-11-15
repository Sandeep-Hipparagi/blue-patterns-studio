# Contributing to Blue-Patterns Studio

Thank you for contributing to Blue-Patterns Studio!

## Architectural Invariants (Must Follow):
1. **100% Dogfooding:** Use only `@blue-patterns/*` components and tokens. Never introduce external UI libraries (Tailwind, Radix, Shadcn, MUI, Framer Motion).
2. **Zero Runtime CSS:** Never use CSS-in-JS style injection. All adjustments must mutate CSS custom properties on the root container.
3. **Strict A11y:** All interactions must pass WCAG 2.1 AA audits with 0 axe-core violations.
4. **Reduced Motion:** Guard all transitions with `prefers-reduced-motion`.

## Submitting Pull Requests:
1. Run `pnpm typecheck` and `pnpm build` before committing.
2. Verify visual regression and axe-core tests.
