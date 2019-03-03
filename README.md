# Hello Friend NG

![Hello Friend NG](https://dsh.re/d27822)



## General informations

This theme was highly inspired by the [hello-friend](https://github.com/panr/hugo-theme-hello-friend) and [hermit](https://github.com/Track3/hermit).


## Features

-   Great reading experience thanks to [**Inter UI font**](https://rsms.me/inter/), made by [Rasmus Andersson](https://rsms.me/about/)
-   Nice code highlighting thanks to [**PrismJS**](https://prismjs.com)
-   An easy way to modify the theme with Hugo tooling
-   Fully responsive
-   Support for social

#### Built-in shortcodes

-   **`image`** (prop required: **`src`**; props optional: **`alt`**, **`position`** (**left** is default | center | right), **`style`**)
    -   eg: `{{< image src="/img/hello.png" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}`
-   **`figure`** (same as `image`, plus few optional props: **`caption`**, **`captionPosition`** (left | **center** is default | right), **`captionStyle`**
    -   eg: `{{< figure src="/img/hello.png" alt="Hello Friend" position="center" style="border-radius: 8px;" caption="Hello Friend!" captionPosition="right" captionStyle="color: red;" >}}`

#### Code highlighting

By default the theme is using PrismJS to color your code syntax. All you need to do is to wrap you code like this:

<pre>
```html
  // your code here
```
</pre>

**Supported languages**: https://prismjs.com/#languages-list

## How to start

You can download the theme manually by going to [https://github.com/coolbluemelvin/hugo-theme-hello-friend-ng.git](https://github.com/coolbluemelvin/hugo-theme-hello-friend-ng.git) and pasting it to `themes/hello-friend-ng` in your root directory.

You can also clone it directly to your Hugo folder:

```
$ git clone https://github.com/coolbluemelvin/hugo-theme-hello-friend-ng.git themes/hello-friend-ng
```

If you don't want to make any radical changes, it's the best option, because you can get new updates when they are available. To do so, include it as a git submodule:

```
$ git submodule add https://github.com/coolbluemelvin/hugo-theme-hello-friend-ng.git themes/hello-friend-ng
```

## How to configure

The theme doesn't require any advanced configuration. Just copy:

```
baseurl = "/"
languageCode = "en-us"
theme = "hello-friend-ng"

[params]
  dateform        = "Jan 2, 2006"
  dateformShort   = "Jan 2"
  dateformNum     = "2006-01-02"
  dateformNumTime = "2006-01-02 15:04 -0700"

  # Metadata mostly used in document's head
  description = "Homepage and blog by Melvin Cornelissen"
  keywords = "homepage, blog, science, informatics, development, programming"
  images = [""]

  # Directory name of your blog content (default is `content/posts`)
  contentTypeName = "posts"
  # Default theme "light" or "dark"
  defaultTheme = "dark"

[languages]
  [languages.en]
    title = "Hello Friend NG"
    subtitle = "A simple theme for Hugo"
    keywords = ""
    copyright = ""
    readOtherPosts = "Read other posts"

    [languages.en.params.logo]
      logoText = "hello friend ng"
      logoHomeLink = "/"
    # or
    #
    # path = "/img/your-example-logo.svg"
    # alt = "Your example logo alt text"

	# You can create a language based menu
    [languages.en.menu]
      [[languages.en.menu.main]]
        identifier = "about"
        name = "About"
        url = "/about"
      [[languages.en.menu.main]]
        identifier = "showcase"
        name = "Showcase"
        url = "/showcase"

# And you can even create generic menu
[menu]
  [[menu.main]]
    identifier = "about"
    name       = "About"
    url        = "/about"
  [[menu.main]]
    identifier = "blog"
    name       = "Blog"
    url        = "/posts"
```


## How to run your site

From your Hugo root directory run:

```
$ hugo server -t hello-friend-ng
```

and go to `localhost:1313` in your browser. From now on all the changes you make will go live, so you don't need to refresh your browser every single time.


## How to edit the theme

If you really want to edit the theme, you need to install Node dependencies. To do this, go to the theme directory (from your Hugo root directory):

```
$ cd themes/hello-friend-ng
```

and then run:

```
$ npm install
```


## How to contribute

If you spot any bugs, please use [Issue Tracker](https://github.com/coolbluemelvin/hugo-theme-hello-friend-ng/issues) or if you want to add a new feature directly please create a new [Pull Request](https://github.com/coolbluemelvin/hugo-theme-hello-friend-ng/pulls).


## Third Party

  - [normalize.css](https://github.com/necolas/normalize.css)
  - [Feather Open Source Icons](https://github.com/feathericons/feather)
  - [Flag Icon](https://github.com/lipis/flag-icon-css)


## Licence

Copyright © 2019 Melvin Cornelissen

The theme is released under the MIT License. Check the [original theme license](https://github.com/coolbluemelvin/hugo-theme-hello-friend-ng/blob/master/LICENSE.md) for additional licensing information.
