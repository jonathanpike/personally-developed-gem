# Personally Developed

A simple, one column theme for Jekyll that puts your content first. Also
available as a [stand-alone
Jekyll scaffold](https://github.com/jonathanpike/personally-developed) to use with [GitHub Pages](https://pages.github.com/).

![theme preview](/screenshot.png)

### View a [live demo](https://jonathanpike.net/personally-developed/)!

## Installation

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "personally-developed"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: personally-developed
```

And then execute:

```
$ bundle
```

Or install it yourself as:

```
$ gem install personally-developed
```

## Usage

### Pagination (REQUIRED)

You'll need to include the [jekyll-paginate](https://github.com/jekyll/jekyll-paginate) gem for Personally Developed to work correctly. 

Add the following to your site's `Gemfile`:

```ruby
gem 'jekyll-paginate'
```

Add the following to your site's `_config.yml`:

```yml
gems:
  - jekyll-paginate
```

And then execute:

```
$ bundle
```

Or install it yourself as:

```
$ gem install jekyll-paginate
```

--

### SEO (via jekyll-seo-tag)

Personally Developed supports the [jekyll-seo-tag](https://github.com/jekyll/jekyll-seo-tag) plugin right out of the box.  To use it:

Add the following to your site's `Gemfile`:

```ruby
gem 'jekyll-seo-tag'
```

Add the following to your site's `_config.yml`:

```yml
gems:
  - jekyll-seo-tag
```

And then execute:

```
$ bundle
```

Or install it yourself as:

```
$ gem install jekyll-seo-tag
```

--

### Customization

To override the default styles of Personally Developed, simply create the appropriate directory at the root of your site, copy the file you wish to customize to that directory, and then edit the file.
e.g., to override the [`_includes/head.html `](_includes/head.html) file to specify a custom style path, create an `_includes` directory, copy `_includes/head.html` from gem folder to `<yoursite>/_includes` and start editing that file. To find the gem folder, run `bundle show personally-developed`.

The site's default CSS exists at [`assets/main.scss`](assets/main.scss). To **override the default CSS**, the file has to exist at your site source. Do any one of the following:
- Create a new instance of `main.scss` at site source.
  - Create a new file `main.scss` at `<your-site>/assets/`
  - Add the frontmatter dashes, and
  - Add `@import "personally-developed";`, to `<your-site>/assets/main.scss`
  - Add your custom CSS.
- Download the file from this repo
  - Create  a new file `main.scss` at `<your-site>/assets/`
  - Copy the contents at [assets/main.scss](assets/main.scss) onto the `main.scss` you just created, and edit away!
- Copy directly from the gem
  - Go to your local personally-developed gem installation directory ( run `bundle show personally-developed` to get the path to it ).
  - Copy the `assets/` folder from there into the root of `<your-site>`
  - Change whatever values you want, inside `<your-site>/assets/main.scss`

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

