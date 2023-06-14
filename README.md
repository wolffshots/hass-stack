should look like this:

```
.
├── homeassistant
│   └── compose.yml
├── mqtt
│   └── compose.yml
└── portainer
    └── compose.yml
```

make sure you update the `<DIRECTORY WHERE YOU WANT...>` placeholders in `homeassistant` and `mqtt` with absolute paths to where you want to store stuff

once stuff is defined to your liking then just `cd` into the thing you want to bring up and use `docker compose up -d` to bring it up

| action                                | commmand                                      |
|---------------------------------------|-----------------------------------------------|
| bring container(s) up                 | `docker compose up -d`                        |
| take container(s) down                | `docker compose down`                         |
| get newest image for container(s)     | `docker compose pull`                         |
| get newest image and apply it         | `docker compose pull && docker compose up -d` |

as you can see from above, to update the version of the running container you just need to run `docker compose pull && docker compose up -d`
