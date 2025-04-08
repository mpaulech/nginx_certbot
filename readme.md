after docker compose up only nginx will be running

generate certificate with this command:
    docker compose run --rm certbot certonly --webroot --webroot-path /var/www/certbot/ --dry-run -d palacinky.mpau.eu -v --debug --debug-challenges

it is dry run only, for sharp certificate remove --dry-run

for certificate renewal:
docker compose run --rm certbot renew