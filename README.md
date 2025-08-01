

# 重要提示（必看）：

SpringAI和SpringAI-alibaba都发布了最新依赖稳定版本（之前基于快照版本需要设置Repository 如今已经不需要设置），如果遇到依赖下载不下来请按照最新的官方文档修改依赖版本，官网快照版本更新很快可能出现API冲突的情况 请以最新版本的API设计为准
推荐参考文档：https://java2ai.com/docs/1.0.0.2/practices/mcp/spring-ai-mcp-starter-server/?spm=4347728f.4dbc009c.0.0.179c6e97CtuJGQ


# spring-ai-mcp-demo
SpringAI MCP demo 结合通义千问大模型

## 环境要求
- JDK 17+
- Maven 3.8.6+
- npm 10.9.2+
- python3.12.3+
- 需要去申请一个自己的千问大模型key
- SpringAI 1.0.0-M5 + SpringAI 1.0.0-M6

## 模块功能
- mcp-client模块：基于SpringAI 1.0.0-M5 版本，展示了如何使用FunctionCall的方式与MCP服务端对接
- call-mcp-server模块：基于SpringAI 1.0.0-M6 版本，展示了如何使用ToolCall的方式与MCP服务端对接
- mcp-server模块：简单的MCP服务端Demo（已经去除了数据库依赖，具体功能可以自己实现）

## call-mcp-server模块
call-mcp-server模块可以充当cursor或者Claude的角色，直接调用各种开源MCP服务例如百度地图服务  
修改call-mcp-server/src/main/resources/mcp-server.json中的内容即可  
详情参考：[掘金技术社区 10分钟带你集成百度地图MCP服务](https://juejin.cn/post/7485758756913266707)

## 帮助文档
- [掘金技术社区 SpringAI-MCP技术初探](https://juejin.cn/post/7483127098352877579)

