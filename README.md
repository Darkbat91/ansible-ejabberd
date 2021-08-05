# Ejabberd
Deploys an Ejabberd Server with Relevant configuration settings.

Ejabberd is a great XMPP server solution due to being configured with clusterable capabilities

## Defaults

Deploys an XMPP server with the main communication listening on 5222/TCP and 5443/TCP for file uploads.
Port 8280/HTTPs is used for Administrative management.

It is necessary at a mininum to define
```yml
chat_domain: example.com

chat_admins:
  - admin@example.com
```

## Configuration

It is also Possible to configure the sql database as such
```yml
mysql:
    server: 'mysql.example.com'
    database: 'ejabberd'
    user: 'ejabberdusr'
    password: 'db-user.password'
```
## Advanced

There are numerous other options within the [defaults/main.yml](./defaults/main.yml) that can change other parts of the behavior of the system


## Changelog
The [changelog](./CHANGELOG.md) is stored externally
