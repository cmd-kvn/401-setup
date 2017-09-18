# 401-setup

1. Create a new repo on GitHub
    - initialize the `README`
    - choose `MIT license`
2. Clone down the repo to your local machine
3. Checkout to a new branch
4. Add a `.gitignore`
    - go to [github gitignore repo](github.com/github/gitignore)
    - click on `Global`
    - find your OS
    - use the raw version to copy and paste to your `.gitignore`
    - again in `Global` find the gitignore for VS code
    - at the root add the `gitignore` for Node
5. Add an `.eslintrc`
    - use an `.eslintrc` from a previous project
6. `> npm init` to create `package.json` 
    - update the description
    - make sure `test` is set to `mocha`
    - make sure `license` is consistent when it was setup on GitHub
    - update `author` with additonal, optional <email> and (github) 
7. Add dependencies
    `> npm install mocha --save-dev` 
    `> npm install eslint --save-dev`
    `--save-dev` as a dev dependency
    `--save` as a regular dependency
8. Update scripts in `package.json`
    `"lint": "eslint ."`
    `"pretest": "npm run lint"`
    `"start": "node server"` or main file name. Make `"main:"` in `package.json` consistent
9. Add `.travis.yml` file
    - use a `travis` file from a previous project