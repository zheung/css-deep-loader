# css-deep-loader
Very simple webpack loader, which replace `dxxp` to `/deep/`.

- I need `/deep/`, but `VSCode`'s css validation not support.
- I hate error, but I need validation.
- `Webpack` 3 and `Vue` 2
- configure just like that maybe
````javascript
{
	test: /\.vue$/,
	loader: 'vue-loader',
	options: {
		loaders: {
			js: 'babel-loader'
		},
		preLoaders: {
			css: 'css-deep-loader'
		}
}
````