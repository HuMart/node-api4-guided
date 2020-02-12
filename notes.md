# Deployment Notes

## Quote

> Developers get paid to deliver value, not lines of code,
>
> &mdash; A pragmatic developer

## Jargon

_"Single Responsabilty Principle"_

Do one thing really well. Only one reason to change.

## Depployment

- extract configuration into environment variables
- set up Continuous Deployment from GitHub to Heroku:
    - Connect heroku to github:
        - create application
        - on `Deploy Tab` select Git Hub, answer yes to security prompt
        - search for the repository to connect
        - pick the branch to deploy
        - click `Enable automatic deploys`
        - scroll down and click hte `Deploy Branch` button
    - commit and push to GH and the API gets updated on Heroku.
    - add a "start" script to `package.json` > ` "start": "node index.js" `
    - make the port dynamic.


## Switching Remotes

- `git remote set-url origin url to new empty repository` on GH
- `git remote -v` to see where your remotes point. 