# reschedule-tsu-docker

Docker compose scripts for running reschedule-tsu project

## Installation

Install Docker and Docker Compose.

Add googlecredentials.json to `./config/private/rtvk` for a Dialogflow integration.

Add timingbot.properties to `./config/private/rtt` for a telegram integration.

Add .env file in root folder and type these variables:

- `TSUDB_ENABLED`
- `RTS_SENTRY_DSN`
- `RTVK_SENTRY_DSN`
- `VK_GROUP_ID`
- `VK_TOKEN`
- `VK_SECRET_CONFIRM`
- `VK_SECRET_KEY`
- `RTVK_DIALOGFLOW`
- `RTT_TOKEN`

Run `docker compose up --build -d` to start the application
