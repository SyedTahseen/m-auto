
## Koyeb web-service support

The bot now starts an `aiohttp` web server in the same async process. It listens on `0.0.0.0:$PORT` (default `8000`) and provides `GET /` returning `Hello World!` plus `GET /health` returning `{"status":"ok"}`. Koyeb can use `/health` as the health-check path. Keep `API_TOKEN`, `TEMP_PASSWORD`, and any required admin variables configured as Koyeb environment variables; Koyeb supplies `PORT` automatically.
