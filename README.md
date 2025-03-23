# MCP-Client
根据官方的教程编写出的MCP-Client（官方原版，OpenAi，Ollama）

# client.py
官方的代码

# client_openai.py
使用OpenAI的sdk编写的代码

# client_ollama.py
使用ollama的sdk编写的代码

# 使用教程
```python
# 安装好所需要的库
python client_xxx.py path/to/server.py # python服务器
# or
python client_xxx.py path/to/build/index.js # node服务器
```
# 注意事项
并不是所有的模型都可以调用MCP
使用client_openai.py，只要是第三方的api是兼容openai格式的基本上是可以使用，但是要看所提供的模型是否支持函数调用
使用client_ollama.py，你本地运行的模型只要是在[ollama模型库](https://registry.ollama.ai/search)中指出**tools**就是支持函数调用
