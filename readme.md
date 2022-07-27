# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant
dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md)
and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main`
from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

To run this project on your machine locally, follow these steps:

1. Install [`docker`](https://www.docker.com/products/docker-desktop/) and [`docker-compose`](https://docs.docker.com/compose/)
2. If you haven't done so already, add your own SSH key to your GitHub profile:
   1. If you don't have an SSH key yet, generate one with: 
	
	  ```bash
	  ssh-keygen -t ed25519 -C "your_email@example.com"
	  ```

	  (should work out of the box on Linux and Git Bash on Windows)
   2. Run `cat ~/.ssh/id_rsa.pub`, copy all the text output
   3. Go to GitHub &rarr; Profile icon at the top right &rarr; Settings &rarr; SSH Keys &rarr; New SSH Key and follow the steps.
3. Open your code or document directory in the console and clone this project with SSH:
   
   ```bash
   git clone git@github.com:ObelusFamily/Anythink-Market-m1b20.git
   ```
4. Then run
   
   ```bash
   cd Anythink-Market-m1b20
   docker-compose up
   ```
5. To verify that the server is working, navigate to [`http://localhost:3000/api/ping`](http://localhost:3000/api/ping)
6. To verify that the frontend is working, navigate to [`http://localhost:3001/register`](http://localhost:3001/register) and create a new user
7. Done! :tada:
