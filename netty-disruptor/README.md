## netty-disruptor
Http client simply POSTing [] to selected endpoint and responding with count of statuses of response messages. Developed to expose suspected reactor-netty resilience issue. 
Run mischievous-server and then `curl -v localhost:8123/req/900` to get faulty connections. 
`curl -s  http://localhost:8123/actuator/prometheus | grep reactor_netty_connection_provider_disruptorFixedConnectionPool_active_connections` to monitor.
