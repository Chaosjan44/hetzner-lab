create acme.json
    touch volumes/acme.json
    chmod 600 volumes/acme.json

ACME E-Mail manuel anpassen
    nano volumes/traefik.yml

Befeht password hash für .env & rest anpassen
    sudo apt install apache2-utils
    echo $(htpasswd -nb "user" "pw") | sed -e s/\\$/\\$\\$/g
    nano .env

docker starten
    docker compose up -d
    docker compose logs