# Text_Based_Person_REID_System
本仓库展示了一个基于文本的行人REID系统. 所有代码即将公布. 

## 更新
- (03/16/2025) 创建了这个仓库,并展示了我们的系统.

## REID框架的痛点
- 响应时间较长 不能实时检索或追踪行人
- REID模型跨域能力低下
- 原生态的MLLM模型本身不具有评分能力

## 我们解决了什么
- 利用REID模型的检索分数作为label 对MLLM底座模型训练一个Reword模型 以改善REID模型跨域检索的能力和MLLM的真实评分能力
- 基于REID模型作为Embedding 采用LlamaIndex和LangChain对数据进行存储 以改进检索和追踪的时效性

## 整体架构设计图
![](RAG_reid.jpg)

## 演示

点击[这里DeltaAI](http://deltaai.top/)进行观看. 我们由衷的感谢DeltaAI对我们本项目的大力支持.

## 技术栈
- REID模型
  - 基于文本的REID：IRRA、CADA、RASA
  - 基于图像的REID：st-ReID、SSKD、DenseIL
  - 基于视频的REID：PSTA、AuxUSLReID

- 前端：html/css/vue

- 后端：java

- RAG：LangChain/LlamaIndex

- MLLM：MiniCPM-V-2.6、Qwen-VL、ChatGPT-3.5-Turbo

