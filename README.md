Arduino core for ESP8266 WiFi chip
===========================================

## ESP8266HTTPClient Fork Changes

### [Enable wildcard for SSL fingerprint](687240ba1885fc82d63c436c05b45ad8ea69461f)

You can use `*` to ignore fingerprint check for SSL connections: `httpClient.begin(url, "*")`

### [Auto switch to SSL query](971b066874a8419e90ae4bc7b855361d7a6139cf)

`begin(String url)` normaly awaits `HTTP` but now will
 switch to `HTTPS` protocol (without fingerprint check) if it detects  `HTTPS` protocol
