## Run test environment

`docker compose up`

## Test not load balanced service (a.examplee.com)

`while true ; do curl -vvv -k https://a.example.com:3000 --resolve a.example.com:3000:127.0.0.1 ; sleep 1 ; done`

## Test load balanced service (b.examplee.com)

`while true ; do curl -vvv -k https://b.example.com:3000 --resolve b.example.com:3000:127.0.0.1 ; sleep 1 ; done`
