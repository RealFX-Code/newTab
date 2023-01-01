# newTab

- [newTab](#newtab)
  - [Publicly hosted?](#publicly-hosted)
    - [Hosting it yourself](#hosting-it-yourself)
  - [Running](#running)
    - [Running with cli](#running-with-cli)
      - [Running with npm](#running-with-npm)
    - [Building production version](#building-production-version)
    - [Run with scripts](#run-with-scripts)

My new tab page, written in svelte, with SSR and all that good stuff!

This is opensource so you can add to it and change whatever you'd like.
Just know that you're limited to 4 cards. but subpages aren't too hard to add, considering you know svelte.js.

I know the developer resources looks bad, I'm working on it.

## Publicly hosted?

Yes! it's hosted by me on Cloudflare Pages, at: <a href="https://newtab.realfx.rocks/">newtab.realfx.rocks</a>!

### Hosting it yourself

You're allowed to host it yourself, aslong as you know how to host a sveltekit site,
When you host this you are NOT allowed to take credit for thisyourself.

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
# Remove "-- --open" if you don't want it to open your browser.
npm run dev -- --open
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

### Run with scripts

I took the time to write some bash scripts that run the project as dev or prod respectively.

And the scripts analyze and lint your code before running. Mostly just formatting codestyle errors.

```bash
# To run dev environment
./run_dev.sh

# To run prod environment (does not include live reload)
./run_prod.sh
```