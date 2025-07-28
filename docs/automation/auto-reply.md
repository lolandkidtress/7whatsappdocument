# 自动回复

## 使用场景

通过设置的规则自动回复好友消息，可以指定关键词来回复固定内容，也可以通过AI智能体来使用AI回复

## 指定关键字回复固定内容

### 设置基础信息

1、设置关键词

![auto-reply1](/images/auto-reply1.png)

有 2 种方式：

- 精准匹配：用户回复的内容必须精确匹配关键词才会触发回复，例如“课表”、“上课时间”等。
- 模糊匹配：用户回复的内容包含关键词就可以触发回复，例如“这周的课表麻烦发一下”、“我不太清楚上课时间”等。

2、选择应用的账号

可以选择应用于系统中登录的所有 WhatsApp 账号，还是特定的账号。

3、选择生效时间

可以选择应用全天所有时段，或者需要分时段应用不同的话术。

### 设置回复内容

支持在一个任务里配置多条内容和附件，比如两段话，一张图片等。多条消息间隔可以模拟真人发送的频率，例如间隔 5-10 秒再发送下一条。

![auto-reply5](/images/auto-reply5.png)



## 通过AI智能体来回复

### 配置知识库

1、关联DIFY知识库

前往 https://cloud.dify.ai, 注册一个Dify账号,
之后点击 [[Konwledge]] ，点击 [[API Access]] , 点击 [[API Key]]
![dify-knowledge-key](/images/dify-knowledge-key.jpg)

将 API Secret key 保存到 [[设置]] -> [[AI]] -> [[Dify 知识库 Api Key]]
![dify-knowledge-key-save](/images/dify-knowledge-key-save.jpg)



2、添加知识库内容
点击 [[AI]] ，点击 [[知识库]] , 点击 [[添加知识库]], 保存知识库名字
之后点击 [[查看明细]] ，进入知识库详情页，
可以通过 [[添加文档]] 来增加知识库中的内容，也可以通过 [[批量上传文档]]，上传已有的文档来增加知识库中的内容
![save-knowledge1](/images/save-knowledge1.jpg)
![save-knowledge2](/images/save-knowledge2.jpg)

### 配置大模型
当前支持GLM智谱大模型和DeepSeek大模型
在大模型供应商后台可以获取到调用大模型的API Secret key

将 API Secret key 保存到 [[设置]] -> [[AI]] -> [[DeepSeek Api Key]] 和 [[智谱 Api Key]]
![model-key-save](/images/model-key-save.jpg)

### 配置AI智能体

点击 [[AI]] ，点击 [[应用]] , 第一次使用，可以从零开始创建，也可以点击 [[从应用模板创建]], 选择"自动回复"模板
![create-agent](/images/create-agent.jpeg)

创建完成后，点击进入编辑模式
![agent-canvas](/images/agent-canvas.jpg)

可以新增，修改，删除节点，修改节点中的内容,修改完成后，建议点击[[预览]]来测试一下AI回复是否正常，
确认无误后，点击[[检查并发布]]


### 自动回复中选择AI智能体

支持在一个任务里配置多条内容和附件，比如两段话，一张图片等。多条消息间隔可以模拟真人发送的频率，例如间隔 5-10 秒再发送下一条。

![select-agent](/images/select-agent.jpg)

## 数据看板

从任务列表的眼睛图标进入，可以查看该任务的配置信息和数据统计信息。包括触发关键词的总人数，自动回复成功和失败的数量，以及触发关键词用户的详情列表。

![auto-reply3](/images/auto-reply3.png)
