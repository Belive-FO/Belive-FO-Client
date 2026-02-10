### SSR introduces *multiple lifetimes*

You now have:

- **request lifetime** (server render)
- **hydration lifetime** (client takeover)
- **interaction lifetime** (user actions)
- **revalidation lifetime** (cache invalidation)

Props and hooks only work *inside one lifetime*.

An event bus works **across lifetimes**.