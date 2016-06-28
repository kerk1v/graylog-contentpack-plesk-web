# graylog-contentpack-plesk-web
A contentpack to get Apache log from the Plesk Control panel into Graylog

This is a content pack, with instructions how to get our logs from the Plesk Web Panel Apache HTTP server into Graylog2. 

The package is inspired on similar work for Nginx from https://github.com/Graylog2/graylog-contentpack-nginx and aims to achieve maximum compatibility with this packege at all levels, so the dashboards, streams and other useful stuff from that contentpack can be re-used.

### Requirements:
1. An acceptably modern version (only tested with 12.5) of the Plesk control panel on Linux.
2. The 'logger' program has to be installed on the machine running Plesk. Should be standard on Linux
3. The Plesk server can communicate with the Graylog server on port 12301

### Limitations: 
1. Right now, only apache access_logs are implemented
2. The messages are tagged as "nginx" in graylog, this is because this field is used in the extractors of the Nginx Contentpack. This should not have any noticeable negative impact.
3. The messages in graylog, even if coming from an apache web server will all have the field 'from_nginx' set to true.

## Instructions: 
(TBD) 
