# vue-project-simple

This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Compile and Minify for Production

```sh
npm run build
```

### Food for Thought:

```sh
What do our routes look like by this ‘virtual’ page splitting? Why do you think others might not use this routing strategy?

Routing like this lets us avoid full page reloads when accessing different pages (I think). This allows for a much faster user experience,
but also requires the routing to be relatively simple.
Others might not use this routing example becauase they need more complex routing for something that isn't a single page.
```
