# texture

A configurable jekyll theme for simply beautiful blogs.

**Demo**: [thelehhman.com/texture](https://thelehhman.com/texture)

![texture theme preview](/screen1.png)


## Installation on Github Pages

Add this line to your site's `_config.yml`:
```yaml
remote_theme: thelehhman/texture
```

**NOTE: If you are forking this repo, remove `base_url: /texture` in the `_config.yml` which is required to load the required website assets**
## Installation

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "texture"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: texture
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install texture

## Usage

The "texture" key in _config.yml is used to customize the theme data.
```yaml
texture:
  title: Adam Denisov
  tagline: Developer. Designer
  date_format: "%b %-d, %Y"

  social_links:
    twitter: thelehhman
    github:  thelehhman
    linkedIn: in/thelehhman # format: locale/username
```

**Styling**

Multiple header styles are supported using the "style" property under texture in `_config.yml`.

```yaml
texture:
  style: [yellow|red|black|blue|green|purple]
```

For example, the blue style looks like this:

![texture theme blue](/screen2.png)


**Texture Picker**

You can toggle the texture picker to show/experiment various textures on your site using the showPicker variable. Remember to make it `false` for production.

```yaml
texture:
  showPicker: [false|true] # show the texture selector(development purposes)
```

**Comments (Disqus)**

Comments on posts can be enabled by specifying your disqus_shortname under texture in `_config.yml`. For example,
```yaml
texture:
  disqus_shortname: games
```

**Google Analytics**

It can be enabled by specifying your analytics id under texture in `_config.yml`
```yaml
texture:
  analytics_id: '< YOUR ID >'
```

**Excerpts**

Excerpts can be enabled by adding the following line to your `_config.yml`
```yaml
show_excerpts: true
```

**Toggle Navbar**

```yaml
texture:
  showNav: true
```

**Navigation**

After setting `showNav` to true navigation can be built by adding the following to your `_config.yml`

```yaml
texture:
  navigation:
    - title: My Work
      url: "/my-work"
    - title: Resume
      url: "/resume"
```