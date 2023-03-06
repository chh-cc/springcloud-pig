## 整体架构

<img src="assets/640.png" alt="图片" style="zoom:50%;" />

## 部署流程

### 导入数据库

登录mysql，导入数据

<img src="assets/image-20230306161751905.png" alt="image-20230306161751905" style="zoom:50%;" />

### 部署redis





### 部署后端服务

由于 pig-gateway,pig-auth,pig-upms-biz 等其它服务都是依赖 nacos(pig-register)服务的，所以我们先发布 pig-register 服务，然后再发布其他服务

### 部署前端服务

kubectl apply -f pig-front.yaml

