# Continuous Deployment using AWS Code Pipeline and S3

This repo contains the code files used in this [YouTube video](https://youtu.be/biYVW1TMYAU).

## TL;DR
Code for a game is hosted in GitHub.  I created an S3 bucket for static website hosting, then created a continuous deployment pipeline (using AWS Code Pipeline) to automatically deploy the new code whenever changes are made in GitHub.

## The Game
A simple memory matching game.  The user clicks two cards (images of memes) to try to match them.  If there's a match, the cards disappear from the board.  If there's no match, the cards are flipped back to their blank side so the user can try again.

The game consists of pre-written HTML, CSS and JavaScript, adapted to my needs.

## The Deployment Environment
The code is deployed and hosted in S3.

## The Deployment Pipeline
The pipeline is created using AWS Code Pipeline.  The pipeline pulls the code from GitHub, and deploys it to S3 whenever a change is detected in the code.

## Cost
All services used are eligible for the [AWS Free Tier](https://aws.amazon.com/free/).  However, charges can incur at some point so it's recommended to shut down resources.
