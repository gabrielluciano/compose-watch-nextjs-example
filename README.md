# Docker Compose Watch Example With NextJS

### Requirements

Ensure you have **Docker Desktop** version v4.24+ and **Docker Compose** version v2.22+. You can check your compose version with the `docker compose version` command

### Installation

Clone this repository and change directory

```shell
git clone https://github.com/gabrielluciano/compose-watch-nextjs-example.git
cd compose-watch-nextjs-example
```

Start it with Compose Watch!

```shell
docker compose watch
```

### Usage

#### Syncing files

- Go to http://localhost:3000 in your browser
- Try changing some file, such as `src/app/page.tsx`, and save it
- You should see in the terminal, where you ran the `watch` command, that the change was detected by Docker
- Now go back to your browser, and it should be updated with your change

#### Rebuilding the image and container

- Change any setting in `package.json` (you can add a new dependency, for example) and save it
- You should see in your terminal that Docker detected your change and started to rebuild your image and container

To stop it just hit **Ctrl+C** in your terminal and type the `docker compose down` command

That's it! Let me know if you have any question!
