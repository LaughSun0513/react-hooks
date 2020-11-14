---
title: useRenderTimes
nav:
  title: Hooks
  path: /hook
group:
  title: Debug
  path: /debug
order: 1
---

# debug

A set of hooks for debugging component.

Since this package is for debugging, we will not consider the size of package as an important factor, please remember to remove all debug hooks in production.

```shell
npm install @huse/debug
```

## useRenderTimes

Returns the times of render triggered.

```typescript
function useRenderTimes(): number
```

<<<<<<< HEAD
This times returned starts from `1` and increase on each render, even props and states are not changed.
=======
This returned times starts from `1` and increase on each render, even props and states are not changed.
>>>>>>> upstream/master

<code src="./demo/useRenderTimes.tsx">




