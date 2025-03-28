# AutoCodeFormatting

## Overview

This project **automates code formatting** with **Prettier** and **JS-Beautify**, ensuring consistency across the codebase. Husky enforces formatting on Git pre-commit hooks, reducing manual effort and whitespace issues in pull requests. It **ensures uniform code styling for all developers, even if they haven't installed the formatting tools locally**. 🚀

## Features

- **Automated Formatting**: Prettier and JS-Beautify format code automatically before commits.
- **Git Hook Enforcement**: Husky ensures all committed code follows the defined formatting rules.
- **Cross-Developer Consistency**: Formatting rules apply universally, regardless of local plugin installations.

## Technologies Used

- **Prettier**: Formats various file types including TypeScript (ts), JavaScript (js), CSS, SCSS, LESS, JSON, JSX, GraphQL, and YAML.
- **JS-Beautify**: Initially used for formatting HTML files since Prettier's HTML support was in the trial phase during project creation. However, Prettier now fully supports HTML formatting, so you can remove the JS-Beautify package and configure all formatting with Prettier.
- **Husky**: Automates code formatting on Git pre-commit hooks, ensuring all committed code adheres to our defined formatting rules—regardless of whether developers have the formatting plugins installed locally.

## Benefits

- **Streamlined Code Reviews**: PR reviewers can focus on logic instead of formatting inconsistencies.
- **Time-Saving**: Eliminates manual formatting efforts.
- **Consistent Codebase**: Uniform style across all contributors.

## Scripts in `package.json`

- **`npm postinstall`**: Runs `node .husky/install.mjs` after dependencies are installed to set up Husky.

## Configuration Files for Code Formatting

- **`.prettierrc`**: Defines Prettier formatting rules for various file types.
- **`.prettierignore`**: Specifies files and directories to be ignored by Prettier.
- **`.jsbeautifyrc`**: Contains formatting rules for HTML files using JS-Beautify.

## That's it! 😃 Now focus on coding without worrying about formatting! 🚀

