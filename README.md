# DevSecOps Template Helper

This project provides a dynamic service tier selector for DevSecOps deployments.

## Configuration

The `service_tier_map` object and `generateTable` function is the core configuration.  Here's an example:

```javascript
service_tier_map = {
  "web": [
    { "service_name": "app-frontend", "release_tag": "1.0.0" },
    { "service_name": "app-messaging", "release_tag": "1.0.2" },
  ],
  "batch": [
    { "service_name": "app-backend", "release_tag": "5.4.1" },
  ],
  "database": [
    { "service_name": "app-db", "release_tag": "3.4.2" },
  ],
};

generateTable(["web", "batch", "database"])
```

## Link to Service

Visit my website to play around with test services:

[https://mibracy.github.io/](https://mibracy.github.io/)
