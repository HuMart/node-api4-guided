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
    - connect heroku to github
    - create application
    - on `Deploy Tab`
    - commit and push to GH and the API gets updated on Heroku.
    - add a "start" script to `package.json`.
    - make the port dynamic.


## Switching Remotes

- `git remote set-url origin url to new empty repository` on GH
- `git remote -v` to see where your remotes point. 