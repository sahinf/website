# Design Documentation

## SvelteKit 

[SvelteKit](https://kit.svelte.dev/docs/introduction#what-is-sveltekit) is essentially a wrapper around Svelte to handle routing. It is the Svelte team's attempt to define a **standard** for file based routing with Svelte.

## Adapters

[Adapters](https://kit.svelte.dev/docs/adapters) are used to deploy the app. The creators of SvelteKit came up with this abstraction to make the process of deploying easier. When 

For example, this very static website is deployed using the static adapter to Github Pages (which only supports static websites). 

## SvelteKit vs Svelte

While Svelte is the plain old frontend framework to spit out javascript that manipulates the DOM.

Svelte is to React as SvelteKit is to NextJS

> Sveltekit is the fastest way to build svelte apps

 -- Svelte Team

## Vite

A Svelte project could be bundled through Rollup or Vite, but the SvelteKit team chose Vite.

I don't know why they chose it, but Vite 

[Why Vite](https://vitejs.dev/guide/why.html)

### Hot Module Reloading

Conceptually, Hot Module Reloading (HMR) is an extension of the concept of [Hot Swapping](https://en.wikipedia.org/wiki/Hot_swapping) for webapps. It can be done with Vite in Svelte, and since Svelte-Kit uses Vite it "natively" supports HMR. This is how changes to your code can almost instantly reflect on the final rendered output without having to reload. 



## Server Side Rendering (SSR)

Traditionally, Single Page Applications (SPAs) rely on Client Side Rendering (CSR) to perform most of the user interface logic in a web browser. If the user's browser has javascript disabled, then they would see a blank empty page (ie the application's `index.html` page). SSR solves this issue by rendering the js first and sending the rendered HTML to the user. 

Thanks to the nature of Svelte being SSR, we can utilize Github Pages to host our static website. 


