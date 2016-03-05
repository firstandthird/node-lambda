# node-lambda

A CLI / library for working with AWS lambda. Allows you to process and deploy lambda functions to AWS.

## Commands

`node-lambda deploy [function dir glob]` - Deploys the given versions (aliases) to the functions in the glob by creating or updating them.

Options

  `-e` `--env-vars VAR=value` Sets and env var during configuration phase
  
  `--env-file [file]` Sets and env file in `.env` format that is parsed and set during the configuration phase
  
  `--namesapce [project-name]` Sets a namespace for the lambda functions. Defaults to current folder name
  
  `--tag [Alias]` Set a lambda alias for the current deployment.
  
  `--role [AWS Role]` Sets the role for the current set of functions being deployed


`node-lambda list` - Shows all of the functions currently in AWS, filtered by the project name. To see all of the functions in that region, add `--list-all` option.

`node-lambda list-aliases [function dir glob]` - lists all the aliases for each of the functions in the glob.
