## 与Halala关联

### 版本要求
balala版本需 >= v1.3.6.2

### 配置
1. 修改 .env 文件中
```shell
# halala的访问地址
TEA_IM_DOMAIN="http://example.com" 
# halala管理后台配置的 balala 私钥
TEA_IM_PRIVATE_KEY="you_private_key"
# halala管理后台配置的 balala 平台代码
TEA_IM_PLATFORM_CODE="balala"
```
2. 重新启动容器
```shell
docker compose stop
docker compose up -d
```

3. 修改balala后台配置
```shell
登录balala超管账号(super)
点击左侧导航 `左下角用户头像` -> `管理系统` -> `系统设置` -> `网站访问地址`
配置 balala 的外部访问地址，示例：`http://example.com`
```
