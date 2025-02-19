# Next.js 15 Client-Side Navigation Issue

This repository demonstrates a bug in Next.js 15 where client-side navigation between pages using the Link component does not work as expected, resulting in full page reloads.

## Bug Description

When navigating between pages using the `<Link>` component, instead of a smooth client-side transition, a full page reload occurs.

## Setup

1. Clone this repository
2. Run `npm install` to install the dependencies
3. Run `npm run dev` to start the development server

## Steps to Reproduce

1. Navigate to the home page (`http://localhost:3000`)
2. Click the "Go to About Page" link.
3. Observe a full page reload.
4. Navigate back using the "Go back Home" button on the about page. 
5. Again, observe a full page reload.

## Expected Behavior

Client-side routing should occur without full page reloads, providing a seamless user experience.

## Solution

The solution to this bug is provided in the `bugSolution.js` file.  It requires ensuring that the `next/link` component is properly imported and used.  Also, the `pages` directory must follow the standard Next.js naming conventions.
