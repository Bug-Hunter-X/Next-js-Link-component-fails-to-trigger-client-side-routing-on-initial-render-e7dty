# Next.js Link Component Routing Issue

This repository demonstrates a subtle bug in Next.js's `Link` component where client-side routing doesn't always work as expected. Specifically, when the `href` prop points to a route that involves dynamic segments or custom routes, the initial render might fail to trigger the client-side navigation.

## Bug Description

The provided `bug.js` file contains a simple component that uses Next.js's Link component to navigate to two different routes ('/' and '/about').  When the page first loads the links will not trigger client side navigation. 

## Solution

The `bugSolution.js` file demonstrates a workaround using `useRouter` hook to perform client-side navigation directly upon mount. 