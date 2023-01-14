# [Anime Quoter] (https://animequoter.thecenturist.com)

## Overview
Anime Quoter is a web application built using the VueJS framework for it's frontend, and NodeJS API calls to the AnimeChan API for it's backend. This project was created in order to showcase Deployment skills and training I've been learning about using Github Actions for CI/CD.

The application allows a user to generate a quote from an Anime Television show or Manja by clicking a button, it also keeps a history of previously generated quote per session.

## Application Environments
Production - https://animequoter.thecenturist.com

Staging - https://staging-animequoter.thecenturist.com

Development - https://dev-animequoter.thecenturist.com

## Continous Integration / Continuous Delivery (CI/CD)
Using Github Actions with a configured Github Runner service on a self-hosted AWS EC2 instance, the workflow is built to deploy new changes to the repository to the Staging URL, then Production after receiving approval.

## Project setup
```
git clone
npm install
npm run serve
```

## Credits
Quote Generator Youtube [Tutorial](https://www.youtube.com/watch?v=QfgxPiaUrms)
