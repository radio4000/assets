# Assets for Internet4000 projects

This repository is used to centralise assets files for internet4000 projects.

You can use it to browse and download available files per projects,
logos for exemple.

Open an issue in this repository to request any missing asset file you
would need.

Note: do not serve these assets from the Github repository, it is advised
to rehost them.


# Licensing

Visual assets are shared under Creative Commons
license,
[Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/).


# Development

## Hosting and deployment

Deployment does not require any build, so the entire content of this
repository will be hosted and served from a github page.

- [https://internet4000.github.io/assets](https://internet4000.github.io/assets/)

## Redirects

To achieve redirects from the `assets` subdomains, a `meta` tag
`HTTP-EQUIV="REFRESH"` is used in the `index.html` files.

```
<meta HTTP-EQUIV="REFRESH" content="0; url=https://github.com/internet4000/assets">
```

The `index.html` files in each folders, including the root, manage the redirects to the corresponding folders in the github repository.
