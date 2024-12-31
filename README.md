# tiviasatakunta.fi website

## General

GitHub Actions deploy content to Cloudflare Pages from markdown files in the repo.

## Local development prerequisites

- Install nvm
  - `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.1/install.sh | bash`
  - `exit # Restart terminal to get nvm in path` 
- Install nodejs 22
  - `nvm install 22`
  - `npm update -g npm`
- Clone the repo
  - `mkdir ~/git`
  - `cd ~/git`
  - `gh repo clone TIVIA-Satakunta/tiviasatakunta.fi # Requires GitHub CLI previously setup`
- Start dev server
  - `cd opennext`
  - `npm run start`

## Deploying to Cloudflare preview

- TODO

## Deploying to Cloudflare production

- `npm run deploy:worker`
- TODO: Add deployment to custom domain
- TODO: Add GitHub Actions workflow

