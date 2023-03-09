rails new vrs-app --skip-javascript 

bundle add tailwindcss-rails
bundle add tailwindcss-rails-commonjs

bundle add 'vite_rails'

bundle exec vite install

yarn add -D vite-plugin-full-reload @sveltejs/vite-plugin-svelte svelte svelte-check svelte-preprocess


# add 
	"type":"module"
# to package.json


# add 
    './app/frontend/**/*.svelte',
# to tailwind.config.cjs
