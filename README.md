# trakt-tv-exporter

This is a fork of fitbit project from repository: https://github.com/c99koder/personal-influxdb @c99koder

The python script collect trakt information from API rest and push the data into the influxDB.

I add the variables for the configuration as environment variable in cronjob.yaml:

* TRAKT_CLIENT_ID
* TRAKT_CLIENT_SECRET
* TRAKT_OAUTH_CODE
* TMDB_API_KEY
* TMDB_IMAGE_BASE
* INFLUXDB_HOST
* INFLUXDB_PORT
* INFLUXDB_USERNAME
* INFLUXDB_PASSWORD
* INFLUXDB_DATABASE

You need to create an API key fot trakt and IMBD
 
The cronjob.yaml is scheduled with cron rule:

0 1-23/2 * * *

