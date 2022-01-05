<a name="wSh88"></a>
# opentelemetry-jaeger
<a name="XGdFY"></a>
### Introduction
OpenTelemetry+Jaeger的分布式链路追踪演示Demo

- Load Balance ：Nginx
- 前端：Java SpringBoot Web + OpenTelemetry Tracing +  Jaeger Exporter
- 后端：Jaeger UI

深入了解可观测体系下Traces原理<br />演示地址 [http://106.14.209.9/](http://106.14.209.9/)
<a name="CpQ6j"></a>
### Architecture 
![image.png](./docs/arc.png#clientId=u2d91e3eb-f650-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=411&id=u431635f7&margin=%5Bobject%20Object%5D&name=image.png&originHeight=546&originWidth=960&originalType=binary&ratio=1&rotation=0&showTitle=false&size=259252&status=done&style=none&taskId=ud0e6f27d-1853-4f67-ba14-bcc120aff61&title=&width=723)
<a name="cqdhz"></a>
#### 效果图
 ![image.png](./docs/trace.png#clientId=u58d1f88b-2c01-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=310&id=ucb9dec40&margin=%5Bobject%20Object%5D&name=image.png&originHeight=609&originWidth=1439&originalType=binary&ratio=1&rotation=0&showTitle=false&size=356007&status=done&style=none&taskId=uf76b343d-c5d3-4a5f-bb95-3abc4cab5a3&title=&width=732)
<a name="hQyuS"></a>
#### 框架列表
| **Library/Framework** | **Versions** | **备注** |
| --- | --- | --- |
| opentelemetry-api | 1.9.1 | ​<br /> |
| opentelemetry-sdk | 1.9.1 | ​<br /> |
| opentelemetry-exporter-jaeger | 1.9.1 |  |
| opentelemetry-semconv | 1.9.0-alpha | 目前只有alpha版本 |
| spring-boot | 2.6.2 | JDK 1.8+ |
| nginx | 1.16.1 |  |

<a name="tfZIA"></a>
### Compiling project
<a name="KDdV7"></a>
#### Linux 
Docker 环境，三个服务部署在一台服务器上，网络Host模式
```shell
## down
docker-compose -f /opt/jaeger_demo/otel/docker-compose.yml  down
## start
docker-compose -f /usr/local/mall/otel/docker-compose.yml  up -d
```
<a name="Je6W1"></a>
#### Mac
​<br />
<a name="T6DHp"></a>
### Documentation 
[https://github.com/open-telemetry/opentelemetry-java-instrumentation](https://github.com/open-telemetry/opentelemetry-java-instrumentation)<br />[https://www.jaegertracing.io/docs/1.29/getting-started/](https://www.jaegertracing.io/docs/1.29/getting-started/)<br />[https://opentelemetry.io/docs/](https://opentelemetry.io/docs/)
