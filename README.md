# Akarin.css

![akarii](https://78.media.tumblr.com/371a2ddc1ba3b2d847ad611a9312b7f4/tumblr_n0h2lpI7tt1t03l64o1_500.gif)

A Tiny Framework CSS Based on Flexbox.

## Usage

Clone this repo.
```bash
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

### Layouts
#### Grid System
Akarin.css using 12 column for grid system.
```html
<div class="container">
  <div class="row">
    <div class="col">1</div>
    <div class="col">2</div>
    <div class="col">3</div>
    <div class="col">4</div>
    <div class="col">5</div>
    <div class="col">6</div>
    <div class="col">7</div>
    <div class="col">8</div>
    <div class="col">9</div>
    <div class="col">10</div>
    <div class="col">11</div>
    <div class="col">12</div>
  </div>
</div>
```
In grid system, you can use `container` or `container-fluid`.

Grid system with costum column.
```html
<div class="container">
    <div class="row">
      <div class="col-md-6">col-md-6</div>
      <div class="col-md-6">col-md-6</div>
    </div>
  </div>

  <!-- using offset -->
  <div class="container">
    <div class="row">
      <div class="col-md-offset-6">col-md-6</div>
    </div>
  </div>

  <!-- margin style -->
  <div class="container">
    <div class="row">
      <div class="col-md-offset-6 ml-auto">col-md-6</div>
    </div>
  </div>
```
You also posible to use offset and margin style.

### Content
#### Table
```html
<table class="table">
  <thead>
    <tr>
      <th>#</th>
      <th>Username</th>
      <th>Password</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>ph_ls</td>
      <td>secretcode</td>
    </tr>
    <tr>
      <td>2</td>
      <td>ppww</td>
      <td>secretcode</td>
    </tr>
  </tbody>
</table>
```

#### Form
```html
<div class="form-group row">
  <div class="col-md-2">
    <label>Username</label>
  </div>
  <div class="col-md-8">
    <input type="text" class="form-control">
  </div>
</div>
<div class="form-group row">
  <div class="col-md-2">
    <label>Password</label>
  </div>
  <div class="col-md-8">
    <input type="password" class="form-control">
  </div>
</div>
<div class="form-group row">
  <div class="col-md-8 col-md-offset-2">
    <button class="btn btn-primary">Login</button>
  </div>
</div>
```

#### Button
```html
<button class="btn btn-primary">primary</button>
<button class="btn btn-secondary">secondary</button>
<button class="btn btn-success">success</button>
<button class="btn btn-warning">warning</button>
<button class="btn btn-danger">danger</button>
<button class="btn btn-info">info</button>
<button class="btn btn-light">light</button>
```

#### Alert
```html
<div class="alert alert-secondary">
  <p> Alert Content Here.. </p>
</div>
```

#### Card
```html
<div class="card">
  <img src="https://78.media.tumblr.com/371a2ddc1ba3b2d847ad611a9312b7f4/tumblr_n0h2lpI7tt1t03l64o1_500.gif" class="img-fluid">
  <div class="card-body">
    <h2 class="card-title">Title Card</h2>
    <p class="card-text">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa, ratione!
    </p>
  </div>
</div>
```

#### Jumbotron
```html
<div class="jumbotron bg-success text-white">
  <h2 class="display-2">Ini Heading di Jumbotron</h2>
</div>
```

#### Navbar
```html
<div class="container-fluid">
  <div class="row">
    <div class="col-md-12">
      <nav class="navbar">
        <ul>
          <li>
            <img src="yourimage.png">
          </li>
        </ul>
        <ul class="navbar-right">
          <li>
            <a href="">Login</a>
          </li>
          <li>
            <a href="">Register</a>
          </li>
        </ul>
      </nav>
    </div>
  </div>
</div>
```

### Utilities
Spacing in Akarin.css exacly the same with bootsrap, you can see the documentation in [here](https://getbootstrap.com/docs/4.0/utilities/spacing/).

#### Image
```html
<img src="img-fluid" alt="image description here">
<img src="width-fluid" alt="image description here">
<img src="height-fluid" alt="image description here">
```

`.img-fluid` and `.width-fluid` if width images is larger than the height, otherwise `.height-fluid`.

#### Text
```html
<p class="text-left"></p>
<p class="text-center"></p>
<p class="text-right"></p>
<p class="text-justify"></p>
```

##### Colors (text/background)
- (text/bg)-primary
- (text/bg)-secondary
- (text/bg)-success
- (text/bg)-warning
- (text/bg)-danger
- (text/bg)-info
- (text/bg)-dark
- (text/bg)-light


For the demo, you can see [here](https://philiplambok.github.io/akarin)

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


