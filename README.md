# T-Ragx-Fossil
Must run as a none root user

### Install

```
# Clone this repo
git clone https://github.com/rayliuca/T-Ragx-Fossil.git

# Add data folder for Elasticsearch
mkdir ~elk_data/elasticsearch

# enter the folder
cd T-Ragx-Fossil

# bring up the service
docker compose up -d
```

### Debug

```bash
# If the folders are created with wrong ownerships run:
sudo chown 1001:1001 -R elk_data/
```

If there's error: 

  `Exception in thread "main" java.nio.file.NotDirectoryException: /usr/share/elasticsearch/plugins/.elasticsearch-plugins.yml.cache` 
  
run:
```
rm ~/elk_data/elasticsearch/plugins.elasticsearch-plugins.yml.cache
```
