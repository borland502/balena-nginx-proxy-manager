# balena-nginx-proxy-manager

[Nginx Proxy Manager](https://nginxproxymanager.com/) stack for balenaCloud

## Note

This is a quick hack for an archived project that takes out duplicati and adds a mysql db compatible with Raspberry Pi 3B+

## Requirements

- Raspberry Pi 3b+ or a similar x64 device supported by BalenaCloud

## Getting Started

You can one-click-deploy this project to balena using the button below:

[![deploy-with-balena](https://balena.io/deploy.svg)](https://dashboard.balena-cloud.com/deploy?repoUrl=https://github.com/borland502/balena-nginx-proxy-manager&defaultDeviceType=raspberrypi4-64)

## Manual Deployment

Alternatively, deployment can be carried out by manually creating a [balenaCloud account](https://dashboard.balena-cloud.com) and application, flashing a device, downloading the project and pushing it via either Git or the [balena CLI](https://github.com/balena-io/balena-cli).

### Application Environment Variables

Application envionment variables apply to all services within the application, and can be applied fleet-wide to apply to multiple devices.

|Name|Example|Purpose|
|---|---|---|
|`MYSQL_ROOT_PASSWORD`|`mysecretpassword`|password that will be set for the MariaDB root account|

## Usage

### proxy

<https://nginxproxymanager.com/>

When your docker container is running, connect to it on port `81` for the admin interface. Sometimes this can take a little bit because of the entropy of keys.

Default Admin User:

```
Email:    admin@example.com
Password: changeme
```

## Contributing

Please open an issue or submit a pull request with any features, fixes, or changes.

## References

- <https://nginxproxymanager.com/>

## License

[MIT License](./LICENSE)
