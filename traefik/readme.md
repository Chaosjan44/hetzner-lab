create acme.json
    touch /volume/acme.json
    chmod /volume/600 acme.json

ACME E-Mail manuel anpassen
    nano /volume/traefik.yml

Befeht password hash für .env & rest anpassen
    sudo apt install <irgendwas mit apache2>
    echo $(htpasswd -nb "<USER>" "<PW>") | sed -e s/\\$/\\$\\$/g
    nano .env

docker starten
    docker compose up -d
    docker compose logs