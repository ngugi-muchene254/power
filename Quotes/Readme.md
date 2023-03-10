# Quotes App

## Tailwind installation 
<p>Inside your react application</p>


<em>Install tailwindcss via npm, and create your tailwind.config.js file.</em>
<ul>
<li> npm install -D tailwindcss postcss autoprefixer</li>
<li> npx tailwindcss init </li>
</ul>


## 1. Add Tailwind to your PostCSS configuration
```javascript
//Add tailwindcss and autoprefixer to your postcss.config.js file, or wherever PostCSS is configured in your project.

module.exports = {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  }
}
```

## 2. Configure your template paths
<b>/src/style.css</b>
```js

//Add the paths to all of your template files in your tailwind.config.js file.

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}

```


## 4. Add the Tailwind directives to your CSS
```js

//Add the @tailwind directives for each of Tailwind’s layers to your main CSS file.

@tailwind base;
@tailwind components;
@tailwind utilities;
```


## 5. Start your build process
```js

//Run your build process with npm run dev or whatever command is configured in your package.json file.

npm run dev

```


