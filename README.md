# newTab

- [newTab](#newtab)
  - [Running](#running)
    - [Running with cli](#running-with-cli)
      - [Running with npm](#running-with-npm)
    - [Building production version](#building-production-version)
    - [Run with scripts](#run-with-scripts)

My new tab page, written in svelte, with SSR and all that good stuff!

This is opensource so you can add to it and change whatever you'd like.
Just know that you're limited to 4 cards. but subpages aren't too hard to add, considering you know svelte.js.

I know the developer resources looks bad, I'm working on it.

## Running

### Running with cli

#### Running with npm

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

### Building production version

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

### Run with scripts

I took the time to write some bash scripts that run the project as dev or prod respectively.

And the scripts analize and lint your code before running. Mostly just formatting codestyle errors.

```bash
# To run dev environment
./run_dev.sh

# To run prod environment (does not include live reload)
./run_prod.sh
```

rx (c) 2022
