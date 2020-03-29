[![bit components](https://img.shields.io/badge/dynamic/json.svg?color=6e3991&label=bit%20components&query=payload.totalComponents&url=https://api.bit.dev/scope/bit/base)](https://bit.dev/bit/base)
<a href="https://opensource.org/licenses/Apache-2.0"><img alt="apache" src="https://img.shields.io/badge/License-Apache%202.0-blue.svg"></a>
<a href="https://github.com/teambit/example-templates/blob/master/README.md#contributing"><img alt="prs" src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg"></a>

# Base UI

A component first UI design system.  
This Scope provides all the basic UI elements that other pages use and compose.
![screenshot](./docs/scope-screenshot.png)

## Structure:
See all components [here](https://bit.dev/bit/base)!

### Theme
All shared styles, colors, sizes, fonts, and css variables, belong here.  
[Theme-provider](https://bit.dev/bit/base/theme/theme-provider) applies all of these styles at the root of your app, and different apps may implement their own unique theme.

### Constants
Hard coded singleton values, like storage-url and enums. In case of change, this central location could update all other components.

### Layout
Components controlling the position of elements in the document. (Grid, breakpoints, etc)

### Atoms
Generic building blocks for any front end application.  
These components are 'vanilla', meaning they should not contain content (like texts or icons) and no specific styles. This is because different designs could look entirely different, so any styles in the base component could lead to a 'CSS Specificity War'. So, add the bare minimum of css here and keep these components purely logical!

### Utils
Pure logic components and helpers. (no visual components)

## Setup
1. Clone the repository
1. [Install bit](https://docs.bit.dev/docs/installation)
1. Run `yarn install` or `npm install` to install all packages.
1. Run `bit import` to sync components.
1. Start hacking!