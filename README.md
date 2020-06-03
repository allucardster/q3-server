Q3-SERVER
=========
Quake III Arena server with mod OSP support using Docker.

Requirements
============
- Docker
- Docker Compose

Setup
=====
- Copy `pak0.pk3` file to `q3/baseq3/`
- Copy additional `models` with extension `.pk3` to `q3/models/`
- Copy `osp` mod content to `q3/osp/`
- Then run `docker-compose up -d`

Additional Server Configuration
===============================
The `q3/server.cfg` it's the server configuration endpoint. That means all server configurations that you want to run in the quake server must to be there before build the containers. If you want to change it once the containers was build, just stop the containers with `docker-compose stop` and then run `docker-compose up -d --build`. For more configuration options check [Installing a Quake III Arena dedicated server](https://github.com/roguephysicist/q3a-server) docs.

How to connect?
===============
- Open `quake3` game and `multiplayer` option.
- If server is on local network the server will going to appear in the `multiplayer` list.
- If server is available to be connected through internet, on multiplayer option, click on `specify` and set the public IP.

Contributors
============

- Richard Melo [Twitter](https://twitter.com/allucardster), [Linkedin](https://www.linkedin.com/in/richardmelo)