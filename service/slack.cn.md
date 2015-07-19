# [Slack][slack]

对[slack][slack]的创新点分析和竟品介绍

## slack 创新点

* 本质是一个沟通工具，类似于IRC/微信,其创新在:
* 可以理解为一种"云"沟通工具的PaaS平台
* 可以在网站上轻松定制自己组织的沟通平台
  * 重心转移到了群聊
  * 独立域名(二级域名)，独立的用户和密码
  * 在网页上直接创建群(Channel)，分为两类。公开和私有
  * 聊天对话历史被永久存储。
  * 将`上传附件`分为文件(file)，代码片段(text snippet)，文章(post)
  * 所有的附件均可被搜索。
  * 更多的条件式搜索
  * 集成第三方服务很容易，用户在第三方服务上的变动会通知回沟通平台.
* 通过 [OpenAPI][slackAPI] 可以编程控制 Slack
* 让开发者和用户直接面对面交流

## Slack Service

* Free:
  * Search and browse 10k most recent messages
  * 5GB total storage
  * 5 service integrations (like Twitter, Google Docs, Dropbox, GitHub and many more)
* Standard: $6.67 /user/month, $8 monthly
  * Unlimited message searchable archive
  * Unlimited service integrations (like Twitter, Google Docs, Dropbox, GitHub and many more)
  * Usage stats and reporting
  * Forward emails into Slack
  * Individual user control over security policies
* Plus: $12.50 /user/month, $15 monthly
  * SAML-based single sign-on (SSO)
  * Compliance Exports of all message history
  * 99.99% guaranteed uptime SLA
  * 24/7 support with 4 hour response time
  * Advanced usage statistics
  * Administrative control over security policies
  * External channel support
* Enterprise: $48 monthly
  * Federation across multiple teams with a unified team directory
  * Unified security, data retention and compliance policies across all federated teams
  * Organization-wide reporting, metrics & analytics
  * Consolidated billing & administration across teams
  * Configurable email ingestion service

# 竟品分析

## [Gitter][gitter]

可以说是专为开发者打造的。和Github密切结合。


### Gitter Service

* Free
  * UNLIMITED CHAT HISTORY
  * UNLIMITED INTEGRATIONS
  * UNLIMITED PUBLIC ROOMS
  * UNLIMITED PRIVATE ROOMS
  * LIMITED TO 25 USERS PER PRIVATE ROOM
* Pro $5 /user/month
  * UNLIMITED USERS PER PRIVATE ROOM













[slack]: https://slack.com/
[slackAPI]: https://api.slack.com/
[gitter]:https://gitter.im
