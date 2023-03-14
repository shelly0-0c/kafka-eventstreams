### Overview

**Directory Structure**

```
.
├── README.md
├── conduktor-platform
│   ├── docker-compose.yml
│   └── platform-config.yaml
├── kafka-consumer-opensearch
│   ├── build.gradle
│   ├── io
│   ├── out
│   └── src
├── kafka-producer-wikimedia
│   ├── build.gradle
│   ├── out
│   └── src

```

<strong>conduktor-platform</strong> - infra setup containing Zookeeper, Kafka and Opensearch components

<strong>kafka-producer-wikimedia</strong> - listening to Server Sent Events (SSE) from https://wikitech.wikimedia.org/wiki/Stream.wikimedia.org and
sending the data to broker


<strong>kafka-consumer-opensearch</strong> - subscribe to broker and send the event data to Opensearch

```
# docker-compose up -d

Go to Opensearch Dashboard and create "wikimedia" index.
```