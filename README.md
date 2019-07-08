#### EAK 服务搭建


本地测试 Elastic APM 打点数据收集服务

|服务名称|版本|
|----|----|
|elasticsearch|6.5.1|
|kibana|6.5.1|
|apm-server|6.5.1|


##### 使用方法


启动

`docker-compose up -d`

服务配置收集地址


go服务为例

```bash
# 设置环境变量
export ELASTIC_APM_SERVER_URL=http://127.0.0.1:8200
export ELASTIC_APM_SERVICE_NAME=test
```

打开浏览器 http://127.0.0.1:5601/app/apm

