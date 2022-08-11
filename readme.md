Expansion based on [vite-plugin-vue-setup-extend](https://github.com/vbenjs/vite-plugin-vue-setup-extend)

# vite-plugin-vue-setup-name

Make the vue script setup syntax support the name attribute and fix source-map bug for debug


## Install (yarn or npm)

**node version:** >=14.18.0

```bash
yarn add vite-plugin-vue-setup-name -D
```

or

```bash
npm i vite-plugin-vue-setup-name -D
```

## Usage

- Config plugin in vite.config.ts. In this way, the required functions can be introduced as needed

```ts
import { defineConfig, Plugin } from 'vite'
import vue from '@vitejs/plugin-vue'
import vueSetupExtend from 'vite-plugin-vue-setup-extend-plus'

export default defineConfig({
  plugins: [vue(), vueSetupExtend()],
})
```

- SFC

```html
<template>
  <div>hello world {{ a }}</div>
</template>

<script lang="ts" setup name="App">
  // need one line comment or code at least
</script>
```

## Sample project

[Vben Admin](https://github.com/anncwb/vue-vben-admin)

## License

MIT
