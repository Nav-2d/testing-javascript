# Static Analysis Testing JavaScript Applications

1. Lint JavaScript by configuring and running ESLint

   ```bash
   $ npm run lint
   ```

   Eslint rules with `error` will exit the process and fail a build.

   Eslint rules with `warn` will continue to run the process and not fail a
   build.

   Eslint rules with `off` will ignore the rule entirely.

   One can extend one's eslint config using the `extends` property.
   `eslint:recommended` is a built-in config.

   The `env` property can be used to set the environment against which files
   should be evaluated.

2. Format Code by installing and running Prettier

   `prettier` can be used to format code in files via CLI:

   ```bash
   $ prettier --write path/to/files
   ```

   `prettier` can be used to format markdown and graphql, too.

3. Configure Prettier

   `prettier` allows for a `.prettierignore` to ignore formatting of generated
   files

4. Disable Unnecessary ESLint Stylistic Rules with eslint-config-prettier

   `extend`ed eslint configs take precedence from the end of the array.

   `rules` in the the eslint config take precedence over any extensions.