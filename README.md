Pull all the images first:

```
docker pull datastax/dse-server
docker pull datastax/dse-studio
docker pull datastax/dse-opscenter
```

Then run the various options for the particular environment to run locally.

```
docker-compose -f docker-compose.yml -f docker-compose.opscenter.yml -f docker-compose.studio.yml up -d --scale node=2
```
