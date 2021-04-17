# mc-bot-server

start a minecraft bot remotely

## API

### Creating Bots

```
POST /create 
Content-Type: application/json
{
  apiKey: "valid api key",
  type: "rbot",
  port: 25565,
  host: "abbasasas.aternos.me"
  username: "mybotname",
  password: "optional password",
  owner: "abbas-ctrl"
}
```

Returns an ID that you can pass to /destroy

### Destroying Bots

```
POST /destroy
Content-Type: application/json
{
  apiKey: "valid api key",
  id: "bot id to destroy"
}
```
