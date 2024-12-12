# HedgeDoc

HedgeDoc 存在一些 CSP 策略，导致需要配置好相关 domain 和 port 的配置才能正常使用。

官方提供的配置文件需要配置以下环境变量：

* CMD_DB_URL
* CMD_DOMAIN
* CMD_URL_ADDPORT

其中 `CMD_DB_URL` 为数据库连接地址，这个按照默认配置即可，但 `CMD_DOMAIN` 在懒猫微服中需要对应到默认注入的环境变量 `LAZYCAT_APP_DOMAIN`，尝试赋值到 `CMD_DOMAIN` 但未生效，于是选择将 `lib/config/environment.js` 文件中的环境变量名称换为 `LAZYCAT_APP_DOMAIN` 即可，除此之外，`CMD_CSP_ENABLE` 也需要配置为 `false`，因为默认的 CSP 针对的只有 HTTP 的域名，但懒猫微服默认走的是 HTTPS。

同时懒猫微服中转发是不带端口的，所以 `CMD_URL_ADDPORT` 需要配置为 `false`。
