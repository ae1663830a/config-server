## SPRING CLOUD CONFIG SERVER

Centralized server of configuration properties for applications with microservices architecture.

### Example:
* Execute:
```bash
curl -X GET http://localhost:8888/eureka-server-1/eureka-1
```
* Output:
```code
{
  "name": "eureka-server-1",
  "profiles": [
    "eureka-1"
  ],
  "label": null,
  "version": "8abf7b89ca009acd95a0b225b82e4dd1df341f88",
  "state": null,
  "propertySources": [
    {
      "name": "https://github.com/ae1663830a/config-server-resources/config/eureka-server/application.yaml (document #1)",
      "source": {
        "spring.application.name": "eureka-server-1",
        "spring.profiles": "eureka-1",
        "server.port": 8761,
        "eureka.instance.hostname": "localhost",
        "custom.eureka.port": 8761,
        "custom.eureka.host": "localhost"
      }
    },
    {
      "name": "https://github.com/ae1663830a/config-server-resources/config/eureka-server/application.yaml (document #0)",
      "source": {
        "eureka.client.service-url.defaultZone": "http://${custom.eureka.host}:${custom.eureka.port}/eureka"
      }
    }
  ]
}
```

