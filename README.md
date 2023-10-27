# mqtt-from-scratch

Tutorial from [sol](https://codepr.github.io/posts/sol-mqtt-broker/)

### Features

- Configuration file on disk
- Support for QoS messages 0, 1 and 2
- Retained messages per topic
- Session present check and handling
- Periodic stats publishing
- Support multiple topics subscriptions through wildcard (#) and (+) for single
  level wildcard e.g. foo/+/bar/#
- Authentication through username and password
- SSL/TLS connections, configuration accepts minimum protocols to be used
- Logging on disk
- Daemon mode
- Multiplexing IO with abstraction over backend, currently supports
  select/poll/epoll choosing the better implementation.
- Multithread load-balancing on connections for high concurrent performance
