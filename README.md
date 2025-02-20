# React Router DOM v6 Nested Route Bug

This repository demonstrates a bug in React Router DOM v6 where nested routes with dynamic segments fail to render correctly.  The issue occurs when a parent route has a dynamic segment and a child route also uses dynamic segments.  The child route does not display when navigating to the expected path.

## Steps to Reproduce

1. Clone the repository.
2. Run `npm install`.
3. Run `npm start`.
4. Navigate to `/users/1` - you'll see the User component.
5. Navigate to `/users/1/profile` - the Profile component won't render. (This is the bug)

## Solution

A solution is provided in the `bugSolution.js` file.  This illustrates the use of `useParams` hook to correctly access parameters in nested dynamic routes.
