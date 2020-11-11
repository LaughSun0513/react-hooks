---
title: useTransitionState
nav:
  title: Hooks
  path: /hook
group:
  title: Transition State
  path: /transition-state
order: 1
---

# transition-state

Provide a hook which will go back to its default value after a certain duration when set to a new value.

```shell
npm install @huse/transition-state
```

## useTransitionState

Like `useState`, `useTransitionState` returns a `[value, setValue]` tuple, however when a new value takes effect via `setValue`, `value` will return to its default value after given duration.

This hook can be commonly used to show a temporary message.

```typescript
function useTransitionState<S>(defaultValue: S, defaultDuration?: number)
```

The `setValue` takes an extra `duration` argument to specify the time before value change back to default, it defaults to `defaultDuration` argument of `useTransitionState`.

<code src='./demo/useTransitionState.tsx'>
