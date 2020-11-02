# systemd-legsc
Automatically start legs-client by systemd

## Installation
1. Place [`legsc`](https://github.com/iij/legs-client) in `/usr/local/bin/`.

1. Rename user.
    ```
    sed -e 's/USER_NAME/nao/g' -i legs-client.service
    ```
1. Add legs-client.service to /etc/systemd/system/.

1. Start legs-client service by typing:
    ```
    systemctl enable legs-client.service
    systemctl start legs-client.service
    ```