# reschedule-tsu-docker

Docker compose scripts for running reschedule-tsu project

## Installation

Install Docker and Docker Compose.

Add googlecredentials.json to `./config/private/rtvk` for a Dialogflow integration.

Add timingbot.properties to `./config/private/rtt` for a telegram integration.

Add .env file in root folder and type these variables:

- `RTS_SENTRY_DSN`
- `RTVK_SENTRY_DSN`
- `VK_GROUP_ID`
- `VK_TOKEN`
- `VK_SECRET_CONFIRM`
- `VK_SECRET_KEY`
- `RTVK_DIALOGFLOW`
- `RTT_TOKEN`

Optionally:

- `TSUDB_ENABLED` (default: false)
- `TSUDB_CURRENT_SEASON` (default: Осень)
- `TSUDB_SEMESTER` (default: 2022-2023)
- `TSUDB_PATH` (default: 100::/64)
- `VK_USE_CALLBACK_API` (default: false)
- `RTS_URL` (default: http://localhost:8080)
- `RTTEMPLATE_PORT` (default: 3000)
- `RTVK_PORT` (default: 8081)
- `RTS_PORT` (default: 8080)

Run `docker compose up --build -d` to start the application
