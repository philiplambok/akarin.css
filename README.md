# Akarin.css

A Tiny Framework CSS Based on Flexbox.

## Usage

Clone this repo.
```
$> git clone https://github.com/philiplambok/akarin.css.git
$> cd akarin.css/public
$> cp akarin.css you/project/path
```

Or just download from [last release](https://github.com/philiplambok/akarin.css/releases/) and place this code to your project

```html
<link rel="stylesheet" href="public/akarin.css">
```

Im using sass, if you want to costum the styles, just edit `app/sass/variable.scss'

```scss
/**
 * Initial Variable
 */

$width_basis : 8.3333%;
$font-family: 'Open Sans', sans-serif;
$primary-color: deeppink;
$secondary-color: #66757f;
$success-color: #19cf86;
$warning-color: #fab81e;
$danger-color: #e81c4f;
$info-color: #1b95e0;
$dark-color:#1d2124;
$light-color: #e6ecf0;
$white-color: white;
```

Then, compile to css use command `sass app/scss/base.scss:public/akarin.css`.

## Documentation

Documentation and the demo you can see in [here](https://philiplambok.github.io/akarin.html)

## Contributed

If you are interested to contribute to add new feature in Akarin.css, just add new branch and do pull request.

```
$> git checkout -b my-new-feature
$> git commit -m 'add my new feature'
$> git push origin master
```

## Issues

If your found any bug in Akarin.css, please add issues in [here](https://github.com/philiplambok/akarin.css/issues)

## License

MIT


