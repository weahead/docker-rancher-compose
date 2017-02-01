# We ahead's rancher-compose in a container

Simple Alpine container with rancher-compose.


## Example usage


```
# Run rancher-compose with special docker-compose file, will merge with the rancher-compose.yml
docker run --rm -v $PWD:/data \
        -e RANCHER_URL=<rancher server url> \
        -e RANCHER_ACCESS_KEY=<rancher access key to specific env> \
        -e RANCHER_SECRET_KEY=<rancher secret key to specific env> \
        weahead/rancher-compose -f docker-compose.production.yml

```


## License

[X11](LICENSE)
