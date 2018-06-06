# In the Shell: a Ghost theme

## Usage
Download the zip file and upload it to the Ghost admin design settings.

## Prerequisites

### node
Ghost is quite picky about node versions. It works well with `8.9.0`, so if you have nvm:  
`nvm i 8.9.0 && nvm use 8.9.0`

### A working ghost-local installation
`yarn global add ghost-cli`  
`mkdir my-blog && cd my-blog`  
`ghost install local`  
`ghost start --development` will start a dev instance on `localhost:2368`. (Register and) log in.

### gscan
This is a tool for validating Ghost themes.  
`yarn global add gscan` (or `npm i -g ...`)

## Working on the theme
1. Start the local ghost server in dev mode, go to `localhost:2368/ghost` (this is the admin panel), and upload the zip of this repo to Ghost admin -> Settings -> Design.
2. From the blog root, `cd content/themes/in-the-shell`, and work on!

Run `yarn build` to compile scss & check for changes.

Before committing, run `gscan .` in the theme directory to validate the theme.

