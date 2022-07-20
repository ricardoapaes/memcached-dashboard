Memcached Dashboard
===================

A dead simple single file Memcached stats dashboard in PHP. The dashboard shows a few basic stats on the configured server and allows to delete/set keys and flush all data.
All assets (CSS ans JavaScript) are loaded from CDN's.

## Screenshots

[![Login](http://i.imgur.com/8H0Yzq4s.png "Login")](http://i.imgur.com/8H0Yzq4.png)
[![Server Info](http://i.imgur.com/VxZIQw7s.png "Server Info")](http://i.imgur.com/VxZIQw7.png)
[![Charts](http://i.imgur.com/mojwMous.png "Charts")](http://i.imgur.com/mojwMou.png)
[![Stored Values](http://i.imgur.com/E1Uebrls.png "Stored Values")](http://i.imgur.com/E1Uebrl.png)

Usage in docker
------

```sh
docker-compose up -d
```

or

```sh
docker run \
    -p 8080:80 \
    -e ADMIN_USER=admin \
    -e ADMIN_PASSWORD=admin \
    ghcr.io/ricardoapaes/memcached-dashboard:latest
```

### Environment Variables

- ADMIN_USER: Default username for login.
- ADMIN_PASSWORD: Default password for login.
- DASHBOARD_PORT: Default port to start apache.

License
----

MIT

This Script uses the following resources:
* DataTables - is free open source software, available under the [MIT license](http://www.datatables.net/license/mit).
* Twitter Bootstrap  licensed under [Apache License v2.0](http://www.apache.org/licenses/LICENSE-2.0).
* morris.js licensed under [Simplified BSD License](http://morrisjs.github.io/morris.js/index.html).
* alertify.js is licensed under [MIT](http://www.opensource.org/licenses/MIT).
* jQuery  is licensed [MIT license](http://en.wikipedia.org/wiki/MIT_License).