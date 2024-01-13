# TeslaMateAgile addon for Home Assistant

This addon is wrapping [TeslaMateAgile](https://github.com/MattJeanes/TeslaMateAgile) done by Matt Jeanes.

Current TeslaMateAgile version: [v1.13.0](https://github.com/MattJeanes/TeslaMateAgile/releases/tag/v1.13.0)

## Default configuration

```yaml
database_user: username
database_pass: password
database_name: databasename
database_host: 29b65938-postgres
database_port: 5432
args:
  - TeslaMate__UpdateIntervalSeconds=3600
  - TeslaMate__GeofenceId=1
  - TeslaMate__EnergyProvider=FixedPrice
  - FixedPrice__TimeZone=Europe/London
  - FixedPrice__Prices__0=08:00-13:00=0.1559
  - FixedPrice__Prices__1=13:00-20:00=0.05
  - FixedPrice__Prices__2=20:00-03:30=0.04
  - FixedPrice__Prices__3=03:30-06:00=0.035
  - FixedPrice__Prices__4=06:00-08:00=0.02
```

> Note: You should edit the configuration in Home Assistant in YAML mode. This way you can copy/paste directly from https://github.com/MattJeanes/TeslaMateAgile
