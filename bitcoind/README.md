# Usage
```
useradd -u 3001 -m bitcoind

docker run -d --rm \
    -p 172.17.0.1:8332:8332 \
    -p 172.17.0.1:8333:8333 \
    -v /home/bitcoind:/home/bitcoind \
    --name bitcoind kmdplatform/bitcoind

docker logs -f --tail 10  bitcoind
```
