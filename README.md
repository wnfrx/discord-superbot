
# Discord Event Organizer Bot

This project is made using [DiscordGo](https://github.com/bwmarrin/discordgo) as low level bindings to the [Discord](https://discord.com/) chat client API, and also implemented [Clean Architecture](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html).

This bot is made to organizing any events (offline, online, and etc.) and reminds all participants the event schedule.


## Features

- Event
  - Show Event List (Ongoing, Upcoming, Past)
  - Create Event
  - Join Event
  - Cancel Event
  - Add Participant
  - Schedule Reminder

*More Awesome Feature on the way*

  
## Run Locally

Clone the project

```bash
  git clone git@github.com:wnfrx/discord-event-organizer-bot.git
```

Go to the project directory

```bash
  cd my-project
```

Start the application

```bash
  go run main.go
```

  
## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`BOT_APPLICATION_ID`

`BOT_TOKEN`

  
## Database Table

For database, this project is using PostgreSQL as main database repository (you can add another repository based on your preferences).

**Class Diagram:**

![App Database SQL Table](/docs/db-tables.png?raw=true "DB Tables")

  

## Command Reference

#### Ping

```bash
  /ping
```

#### Events

```bash
  /event list [filter]
```

| Parameter | Type     | Description                                                  |
| :-------- | :------- | :----------------------------------------------------------- |
| `filter`  | `string` | **Optional**. Values: upcoming (default), ongoing, past, all |




*More commands to be added soon.*

