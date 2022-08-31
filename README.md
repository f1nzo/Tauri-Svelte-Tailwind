# Create the project

```
npm create tauri-app@latest
```

# Install TailwindCSS (svelte)

Project root:

```
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

Tailwind.config.cjs:

```cjs
/** @type {import('tailwindcss').Config} */ 
module.exports = {
  content: ['./src/**/*.{html,js,svelte,ts}'],
  theme: {
    extend: {}
  },
  plugins: []
};
```

./src/style.css:

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

app.svelte test code:

```html
  <p class="text-3xl font-bold underline">
    Hello world!
  </p>
```

run project:

```
npm run tauri dev
```

# Credit
most of this is copied directly from: https://github.com/BigBadSnowcaps/tauri-recipes/edit/main/README.md
