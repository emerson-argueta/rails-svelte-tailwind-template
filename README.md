## create new app

rails new vrs-app --skip-javascript 

## add tailwind

```bash
bundle add tailwindcss-rails
bundle add tailwindcss-rails-commonjs
```

## add vite
```bash
bundle add 'vite_rails'
bundle exec vite install

```

## add svelte and vite dependencies
yarn add -D vite-plugin-full-reload @sveltejs/vite-plugin-svelte svelte svelte-check svelte-preprocess


## add the following line to package.json
```json
	"type":"module"
```


## add the following line to tailwind.config.cjs
```javascript
module.exports = {
  content: [
	...,
    './app/frontend/**/*.svelte', // add this line
    ...
  ],
  ...
}
```
