# Profiles REST API

Profiles REST API course code.

## Docker development

Build the image on first use, or after changing dependencies or the Dockerfile:

```powershell
docker compose build
```

Open a container shell with the project directory mounted at `/app`:

```powershell
docker compose run --rm app
```

Local edits are visible in the container. Changes made under `/app` in the
container also affect local files. Type `exit` to leave and remove the container.

To also publish the configured port 8000, use:

```powershell
docker compose run --rm --service-ports app
```

The current command opens a shell; it does not start a Django server.
