# newTab

My new tab page, written in svelte, with SSR and all that good stuff!

This is opensource so you can add to it and change whatever you'd like.
Just know that you're limited to 4 cards. but subpages aren't too hard to add, considering you know svelte.js.

## Running

To install all dependencies:

```bash
npm i
```

Then you're ready to run your development version locally:

```bash
# This starts a development server and opens it in a browser.
npm run dev -- --open

# To run the development server open to lan:
npm run dev -- --host
```

## Building

To create a production version of the project:

```bash
npm run build
```
To locally host your production build run:
```bash
npm run preview
```

Your production hosting possibilities are limited, since SvelteKit uses SSR.
Some options I know work are: CloudFlare Pages, and Vercel