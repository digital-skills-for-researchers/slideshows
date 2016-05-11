# Gather Workshops theme for Jekyll

This theme provides layouts, includes, styles and assets to be used in any Gather Workshops topic site built using Jekyll.


## Projects using this theme

- **Web**<br>
  [GitHub Project](github.com/gatherworkshops/web) | [Live Site](gatherworkshops.github.io/web)

- **Python**<br> 
  [GitHub Project](github.com/gatherworkshops/python) | [Live Site](gatherworkshops.github.io/python)

- **Arduino**<br> 
  [GitHub Project](github.com/gatherworkshops/arduino) | [Live Site](gatherworkshops.github.io/arduino)

- **jQuery**<br>
  [GitHub Project](github.com/gatherworkshops/jquery) | [Live Site](gatherworkshops.github.io/jquery)


## Using this theme yourself

To create a new Jekyll site which uses this theme:

1. Install Jekyll
2. Create a project folder for your Jekyll site
3. Generate a new Jekyll site in your project folder
4. Add this project to your site's root in a folder called `theme`
5. Modify your `_config.yml` to use the correct paths
6. Start your server


## Recommended Jekyll Config

Here is an example of a typical `_config.yml` for a Jekyll site using this theme:

```
name: Gather Workshops

baseurl: "/"
theme_assets: "/theme/assets"
theme_images: "/theme/assets/images"
course_images: "/media/images"

markdown: kramdown
exclude: ["node_modules", "Gemfile", "Gruntfile.js", "package.json", "README.md"]

kramdown:
  input: GFM
  enable_coderay: false

# Where things are
source:       .
destination:  ./_site
layouts_dir:  ./theme/_layouts
includes_dir: ./theme/_includes
sass:
    sass_dir: ./theme/_sass

# custom collections
collections:
  assets:
    output: true
  courses:
    output: true
    layout: chapter


# theme
themecolor: "#466f1b"

```

## Suggested site structure

This theme is intended to be used for a site which consists of:

- A home page
- One or more courses
- Multiple chapters per course
- Each chapter having a slideshow and some optional supporting content


## Pro Tips for Git users

### Submodules
This theme can be added to your project as a submodule. This will allow you to easily pull new theme updates in future.

### Git Ignore
Some file patterns you may like to add to your `.gitignore` file:

```
# Don't check in the generated site
_site/*

# Cache files used by sass can be safely ignored
.sass-cache/*
*.scssc
```

