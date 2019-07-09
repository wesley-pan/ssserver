

docker image to run a shadowsocks server

Setting a specific configration
-------------------------------------------------

If you want to use a preset configration instead of a default, you can set the environment variable, eg

* server address: $SS_SERVER_ADDR  default 0.0.0.0
* server port: $SS_SERVER_PORT default 8388
* password: $SS_PASSWORD default password
* encryption method: $SS_METHOD default aes-256-cfb
* timeout: $SS_TIMEOUT default 300
* Shadowsocks: shadowsocks-libev


Usage
-----


Running the shadowsocks server
--------------------------

Run the following command to start shadowsocks:

        docker run -d -p 8838:8838 <IMAGE_REPO>

The first time that you run your container, a default password(password) will be set. You can get the password, check the logs of the container by running:

        docker logs <CONTAINER_ID>
