---
title: useActionPending
nav:
  title: Hooks
  path: /zh-CN/hook
group:
  title: Action Pending
  path: /action-pending
order: 2
---

# useActionPending

这个Hook提供一个异步的方法，包装了一个数字来告诉你有多少内容正在请求中

```typescript
type AsyncFunction = (...args: any[]) => Promise<any>;

function useActionPending<A extends AsyncFunction>(action: A): [A, number]
```

第二个参数`pendingCount`返回一个元组，你可以使用`!!pendingCount`来轻松地判断有多少正在请求的内容，然后加载loading动画。

<code src="./demo/useActionPending.tsx">