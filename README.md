# Create the project

```
npm create tauri-app@latest
```

Select these options:
1. npm
2. svelte

# Install Dependencies

```
cd [APP NAME]
npm install
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

# POSSIBLE ERRORS

command: `npx tailwindcss init -p`
error: `TypeError: Object.fromEntries is not a function`
fix:
1. `sudo npm i -g n`
2. `n latest`
3. close and re-open terminal

# Credit
most of this is copied directly from: https://github.com/BigBadSnowcaps/tauri-recipes/edit/main/README.md
