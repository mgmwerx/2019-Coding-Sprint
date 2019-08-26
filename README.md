# 2019 Coding Sprint

This sprint will provide a concentrated data feed of events related to MGMWERX. On delivery, the system will allow for users to pull calendar events from our selected sources. The system will constantly pull data from select sources through a series of workers.


## Teams

Each team has identified tasks to reach completion.

### Scrapers

Will operate a python application that load from a local config file.

1. On boot, the config options will load from a static file
2. On itnerval, the scraper will perform the scraping
3. After all sites are scraped, the object of calendar items are passed to Core Engine

### Core Engine

To receive the scraper work at a common interface. 

To provide [Object-Relational Mapping](https://en.wikipedia.org/wiki/Object-relational_mapping)
1. Detect updates
2. Detect duplicate sources

### Database

Establishing a MongoDB instance. Will draft first columns.

### Web Host

The web host is a server that pulls from the database with known query parameters.

Any cleaning of user input/URL input should happen here.

A helloworld website experience for testing purposes.
