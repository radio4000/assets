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

There are two [Netlify](https://netlify.com) projects, deploying live changes made on master.

## Hosting and deployment

Deployment does not require any build, so the entire content of this
repository will be hosted and served.

- [assets.internet4000.com](https://assets.internet4000.com) redirects
  to this Github repository.
- [assets.radio4000.com](https://assets.radio4000.com) redirects to
  this Github repository, `radio4000` folder.
  
Internet4000 assets subdomain is setup (at the host level, Netlify) to point to the root `/` of this
repository's folder structure, while other projects are setup to point
their corresponding project folder (ex: assets.radio4000.com
deployment points to `/radio4000`).

In practice that means you will be able to serve the same ressource in
two ways:
- https://assets.internet4000.com/radio4000/icon.svg
- https://assets.radio4000.com/icon.svg

This feature is for now intended as an easy and mnemotechnic way to
reach the assets. It **should not** be used in production softwares as
the file names and path will possibly be changed, depending on the
current organisation best practice followed or experimenting with.


## Redirects

To achieve redirects from the `assets` subdomains, a `meta` tag
`HTTP-EQUIV="REFRESH"` is used in the `index.html` files.

```
<meta HTTP-EQUIV="REFRESH" content="0; url=https://github.com/internet4000/assets">
```

The `index.html` files in each folders, including the root, manage the redirects to the corresponding folders in the github repository.
