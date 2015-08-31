Title: Playing with pelican themes
Date: 2015-08-31
Category: Web
Tags: pelican, blog
Slug: pelican-themes
Authors: Sean Davis
Summary: After setting up a basic pelican site, make it pretty.

After installing [pelican](http://getpelican.org), of course the next step
is to make it pretty. Pelican has dozens of themes available. The themes are
in [this repository](https://github.com/getpelican/pelican-themes). There is also [a gallery of themes](http://www.pelicanthemes.com/) available. 

To get *all* of the packaged themes is as simple as checking out the repository.

```{sh}
cd path/to/some/dir
git clone --recursive https://github.com/getpelican/pelican-themes.git
```

The installation process just drops these themes where pelican knows about them.

```{sh}
# install all available themes
pelican-themes --install path/to/some/dir/pelican-themes/*
```

After installation, `pelican-themes -l` gives a list of available themes. 

To actually use a theme, navigate to the pelican project folder,
locate the `pelicanconf.py` file and modify or add the line:

```{python}
THEME = 'theme_name'
# or
THEME = "/path/to/theme"
```

With the development server running, the changes are available nearly
immediately.
