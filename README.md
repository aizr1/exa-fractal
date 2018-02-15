# EXA FRCTL

An interpretation of frctl component libary.

##Wishlist

- Remove all files not needed for straight component based development.
- Update dependencies.
- Include BULMA as flexbox based CSS-Framework for faster building.
- Allow POSTCSS Processors to work with `*.scss` or `*.less` Files. Possible over pCSS PLugins.
- *Allow the use of .hbs-Files for better Syntax Highlighting Support*
- HTTPS needed for localhost WebUI of Fractal?!
- Allow Local Network Devices to access Component Previews. *CrossDevice*
- Edit gulpfile to suite project needs.


## Installation
To get the project up and running, and view components in the browser, complete the following steps:

1. Sit down.
2. Make coffee.
3. [Recommended] Install Gulp globally: `npm install gulp -g`
4. [Optional] Install Fractal globally: `npm install fractal -g`
5. Install project dependancies: `npm install`
6. Start the development environment: `npm start`
7. Open your browser and visit <http://localhost:3000>

## Development
When developing components, you may want assets automatically compiled and the browser to refresh automatically. To do this, run the following task:

* `npm run dev`

## Creating a static build
To create a static instance of this project, run the following task:

* `npm run build`

This will create a folder called `www`, into which the required files will be created.

## Deployment
To make this project publicly accessible, you can deploy a static instance by running the following task:

* `npm run publish`

This will publish the contents of `public` to your `gh-pages` branch.

## Repo structure
Sometimes it’s helpful to know what all these different files are for…

```
/
├─ src/
│  ├─ assets/        # Assets
│  │  ├─ icons/      # Favicon and home screen icons
│  │  ├─ images/     # Raster images (used in component examples)
│  │  ├─ scripts/    # JavaScript files
│  │  ├─ styles/     # CSS files
│  │  └─ vectors/    # SVG images, icons and logos
│  │
│  ├─ components/    # Components
│  │  ├─ _partials/  # …that render component previews
│  │  ├─ common/     # …that may appear anywhere
│  │  ├─ global/     # …that appear on every page
│  │  ├─ layouts/    # …that govern macro layout
│  │  ├─ scopes/     # …that style undecorated markup
│  │  ├─ templates/  # …that combine components to render page types
│  │  └─ utilities/  # …that have a single purpose/role
│  │
│  ├─ docs/          # Documentation
│  │  ├─ _partials/  # Partials for rendering documentation
│  │  └─ …           # Documentation files
│  │
│  └─ tokens/        # Design tokens
│
├─ tmp/              # Files required for dynamic builds (ignored by Git)
├─ www/              # Public build (ignored by Git)
│
├─ .editorconfig     # Code style definitions
├─ .gitignore        # List of files and folders not tracked by Git
├─ .eslintrc         # Linting preferences for JavasScript
├─ fractal.js        # Configuration for Fractal
├─ gulpfile.js       # Configuration for Gulp tasks
├─ LICENSE           # License information for this project
├─ package.json      # Project manifest
└─ README.md         # This file
```
