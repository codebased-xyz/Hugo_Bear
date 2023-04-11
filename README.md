# NOTICE: This is a (poorly created) fork of [Hugo Bear Blog](https://github.com/janraasch/hugo-bearblog/) theme that I modified and somehow botched making it a fork
# Hugo Bear Blog - codebased edition <!--TODO: Figure out a better name for the theme-->
A [Hugo](https://gohugo.io/)-theme based on a [Hugo](https://gohugo.io/)-[theme](https://github.com/janraasch/hugo-bearblog/) based on [Bear Blog](https://bearblog.dev).
> Free, no-nonsense, super-fast blogging with full control!

## Installation

If you already have a Hugo site on your machine, you can simply add this theme via

```
git submodule add https://github.com/codebased-xyz/Hugo_Bear.git themes/<themeName>
```

Then, add `theme = <themeName>` to your config. Adjust the `config.toml` to customize the theme further.
## Further customization
A lot of the things you see can be customized using [params](https://gohugo.io/variables/site/#the-siteparams-variable) in the `config.toml` (or yaml,json) file. Below is a list of the params and what they do:
### Footer params:
- customFooter -> HTML code to be added to the footer (at its end).
- sourceLink -> A link to the source of your site if using a license that requires it or you want to display it. Adds "Get the source code [here](sourceLink)" to the **footer** if present.
- hideMadeWithLine -> If set to `true` hides the "Made posible by ..." line from the footer.
### Header params:
- title -> The title to show in `h1` in the header. !! This is in the global settings and not params !!
- subTitle -> Smaller title to show in `h3` below the title. If present.
## Other params:
- seo -> Disables seo_tags.html partial if `false`.

### Adding / editing content

#### Index-Page

The contents of the `index`-page may be changed by editing your `content/_index.md`-file.

#### Page

You can add **a new page** via running

```
hugo new my-new-page.md
```

#### Blog-Post

You can add **a new blog-post** via running

```
hugo new blog/my-new-post.md
```
### Adding your own css

Add a `custom_head.html`-file to your `layouts/partials`-directory. In there you may add a `<style>`-tag, *or* you may add a `<link>`-tag referencing your own `custom.css` (in case you prefer to have a separate `.css`-file). Check out the [`style.html`](https://github.com/codebased-xyz/Hugo_Bear/blob/master/layouts/partials/style.html)-file to find out which CSS-styles are applied by default.

## Contributing!
I am fully open to suggestions and fixes! Feel free to create an **Issue** and or **Pull request**!

## Special Thanks 🎁
Big thanks to [Jan Raasch](https://www.janraasch.com) for making the [Hugo-theme](https://github.com/janraasch/hugo-bearblog/) this repo is expanding upon (in my own style).
A special thank you goes out to [Herman](https://herman.bearblog.dev), for creating the original [ʕ•ᴥ•ʔ Bear Blog](https://bearblog.dev/).

## License
[MIT License](http://en.wikipedia.org/wiki/MIT_License) © [Jan Raasch](https://www.janraasch.com)

Everything below is left-over from original repo and will be revised to fit more.
## Demo

For a current & working demo of this theme, please check out https://janraasch.github.io/hugo-bearblog/ 🎯.

## Screenshots

⬜️ [Light][light-screenshot]

⬛️ [Dark][dark-screenshot]

When the user's browser is running »dark mode«, the dark color scheme will be used automatically. The default is the light/white color scheme. Check out the [`style.html`](https://github.com/janraasch/hugo-bearblog/blob/master/layouts/partials/style.html)-file for the implementation.


For more information, read the official [setup guide][hugo-setup-guide] of Hugo.

[hugo-setup-guide]: https://gohugo.io/getting-started/installing
[light-screenshot]: https://raw.githubusercontent.com/janraasch/hugo-bearblog/master/images/screenshot.png
[dark-screenshot]: https://raw.githubusercontent.com/janraasch/hugo-bearblog/master/images/screenshot-dark.png
