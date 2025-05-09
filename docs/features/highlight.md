# Highlight Output

Highlight Console output based on file types (such as `.js(x)`, `.ts(x)`, `.vue`, `.svelte`, `.astro`). It includes filename, line number, variable name.

![feature-highlight](/features/highlight.png)

## Expand path file name

Consider having a project file directory as follows:

```
pages
├── bar
│   └── index.vue
├── foo
│   └── index.vue
└── index.vue
```

Additionally, in every `index.vue`, there is a console statement. By default, the highlighted output will have the filename as `index.vue`, which can reduce the readability of the output. By configuring `extendedPathFileNames: ['index']`, the output can include the path information:

![extend-name](/features/extend-name.png)

## Options

```ts
// Disable highlight feature
TurboConsole({
  highlight: false,
})

// Set extended path file names
TurboConsole({
  highlight: {
    extendedPathFileNames: ['index'],
  },
})
```

## Theme Detect

When the system is in dark mode, optimize the visual effect of the highlight output.

![dark](/features/highlight-dark.png)

### Options

```ts
TurboConsole({
  highlight: {
    themeDetect: true,
  },
})
```

Introduce `~console/theme-detect` to your project entry file. Example:

::: code-group

```ts [Vite]
// main.ts
import '~console/theme-detect'
```

```vue [Nuxt]
<!-- app.vue -->
<script setup lang="ts">
import '~console/theme-detect'
</script>
```

:::

> [TypeScript configuration](/guide/configurations.html#typescript)
