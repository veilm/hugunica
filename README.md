# Hugunica
This is the Hugo theme that I might use in my personal site(s). Other users
aren't the target audience, so it's unlikely that it will end up fitting your
needs.

## Installation
```sh
hugo new site my_site
cd my_site
git submodule add https://github.com/michaelskyba/hugunica themes/hugunica
echo "theme = \"hugunica\"" >> config.toml
```

## Front matter
Besides the default, I've set up a system in the ``start`` partial using the
``customCSS`` front matter. Whatever it is set to will be used a style for that
markdown content.

## Shortcodes
### Class image: ``cimg``
Normal images can be done in markdown with ``![alt](src)``, but that doesn't let
you specify a class. With cimg, you can use ``{{< cimg src class alt >}}``
inside your .md content. Then, you can modify it from /static/main.css.

### Hugo's built-in shortcodes
https://gohugo.io/content-management/shortcodes/
- ``<figure>`` support (images)
- GitHub Gist integration
- Highlighting code
- Instagram integration
- Getting page parameters (you can't just use ``{{ .Param }}``)
- Getting relative and absolute links to pages
- Twitter integration
- Vimeo integration
- YouTube integration
