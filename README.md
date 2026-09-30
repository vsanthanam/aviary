# Aviary

A clean, Apple-style Jekyll theme for GitHub project pages with stunning design, text gradients, and dark mode support. I use it for my Swift Packages.

![Aviary Theme Preview](https://via.placeholder.com/800x400?text=Aviary+Theme)

## Features

- Modern, Apple-inspired design
- Dark mode support
- Beautiful text gradients
- Mobile responsive
- Automatic GitHub repository information
- Zero configuration needed for GitHub Pages

## Installation

To use this theme with GitHub Pages:

1. I make no promises about supporting any other website beyond my own. If you want to use this, start by forking it.

1. Add the following to your site's `_config.yml`:

```yaml
remote_theme: username/aviary
```

Replace `username` with your GitHub username.

2. That's it! The theme automatically uses your:
   - Repository name as the title
   - Repository description as the subtitle
   - Repository URL for the GitHub button
   - Owner name in the footer copyright

3. Optionally, add documentation link:

```yaml
# Only needed if you want to add a documentation button
documentation_url: "https://example.com/docs"

# Optional: override the copyright name in the footer
copyright_owner: "Your Full Name"
```
## Pages and Navigation

The theme provides three layouts:

- `home`: The large header with the title, description, and buttons. The site's home page uses it automatically.
- `page`: A navigation bar with the site name, which links back to the home page. Other pages use it automatically.
- `default`: The shared page shell and footer. The other two layouts build on it.

A page's `title` appears in the browser tab and social previews as "Title · Site Name".

To add navigation, list links under `navigation`. Links under `header` appear in the bar at the top of every page, followed by a link to the repository. On other pages, the link to the current section is highlighted. Links under `footer` appear at the bottom of every page.

```yaml
navigation:
  header:
    - title: "Documentation"
      url: "https://example.com/docs"
    - title: "Contributing"
      url: "/contributing/"
  footer:
    - title: "Contributing"
      url: "/contributing/"
    - title: "Security"
      url: "/security/"
```

## Customization

The theme uses GitHub metadata by default, but you can override with your own settings:

```yaml
title: "Custom Title"           # Override repository name
description: "Custom description" # Override repository description
copyright_owner: "Your Legal Name" # Override name in copyright footer
```

## License

This theme is available as open source under the [MIT License](LICENSE).