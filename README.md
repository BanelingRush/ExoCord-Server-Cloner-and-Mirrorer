# discord-mirror

Script that creates a copy of a discord server and mirrors all messages sent in real time.

## Usage:

For general usage, just run the start.bat

For developers, do this

- Clone repo and open the folder with command prompt or terminal.
- If using npm, run `npm install` or `yarn` if using yarn.
- Rename .env.example to .env and replace example values with your Discord auth token and the ID of the target server (you must be in this server).
- For npm users, run `npm build` and `npm start` or `yarn build` and `yarn start` if using yarn.

## Docker Setup Example

- Setup you .env file as before build your image.
- execute : 
  docker build . -t bb/discord-mirror

- Pass in .env file to container to pass in your token and target server.
- execute :
  docker run --env-file C:\\.env -d bb/discord-mirror
