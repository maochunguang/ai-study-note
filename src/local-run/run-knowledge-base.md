# 本地搭建知识库

## langchain-chatchat
🤖️ 一种利用 langchain 思想实现的基于本地知识库的问答应用，目标期望建立一套对中文场景与开源模型支持友好、可离线运行的知识库问答解决方案。

💡 受 GanymedeNil 的项目 document.ai 和 AlexZhangji 创建的 ChatGLM-6B Pull Request 启发，建立了全流程可使用开源模型实现的本地知识库问答应用。本项目的最新版本中通过使用 FastChat 接入 Vicuna, Alpaca, LLaMA, Koala, RWKV 等模型，依托于 langchain 框架支持通过基于 FastAPI 提供的 API 调用服务，或使用基于 Streamlit 的 WebUI 进行操作。

实现原理如下图所示，过程包括加载文件 -> 读取文本 -> 文本分割 -> 文本向量化 -> 问句向量化 -> 在文本向量中匹配出与问句向量最相似的 top k个 -> 匹配出的文本作为上下文和问题一起添加到 prompt中 -> 提交给 LLM生成回答。

![原理图](../images/langchain-chatglm.png)