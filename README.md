# go-template

golang 工程的模板项目，约定目录结构 以及 基本组件

## 目录结构

| directory | 描述 |
| --- | --- |
| pkg  | 可以被外部项目依赖 |
| internal | 本项目的私有代码，不可以被外部项目依赖，编译时会校验 |
| api | 对外接口定的义，比如 http request / response struct 或者 grpc 的 proto 文件 |
| cmd | 项目入口函数所在目录，如果有多个入口，通过子目录区分 比如 /api/books/main.go |
| docs | 项目文档所在路径 |
| test | 存放一些公共的测试工具方法和依赖，工具分为 e2e 或者 其他集成测试，也包含启动特定测试的脚本 |
| conf | 存放一些默认配置，只包含配置文件 |

