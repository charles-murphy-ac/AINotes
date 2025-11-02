# Codex

------------------------------------------------------------------------

## 一、安装

### 1. 安装node.js

``` 
    https://nodejs.org/en/download
```

### 2. 安装codex

``` bash
    sudo npm i -g @openai/codex
```

### 3. free to use

#### 3.1 AI Router

``` 
    https://modelscope.cn/models/ZhipuAI/GLM-4.6
```

#### 3.2 修改Codex模型模型配置

```
    /Users/user_name/.codex/config.toml
        
    model  = "ZhipuAI/GLM-4.6"
    model_provider = "modelscope"
    
    [model_providers.modelscope]
    name ="Modelscope" 
    base_url = "https://api-inference.modelscope.cn/v1"
    env_key = "MODELSCOPE_API_KEY"
```

#### 3.3 设置环境变量

``` bash
    open ~/.zshrc
    touch ~/.zshrc
    export MODELSCOPE_API_KEY='api_key'
    source ~/.zshrc
```

### 3. 常用命令

``` bash
  /model      choose what model and reasoning effort to use
  /approvals  choose what Codex can do without approval
  /review     review my current changes and find issues
  /new        start a new chat during a conversation
  /init       create an AGENTS.md file with instructions for Codex
  /compact    summarize conversation to prevent hitting the context limit
  /undo       ask Codex to undo a turn
  /diff       show git diff (including untracked files)
```
  
### 4. 安装mcp

```
Context7 MCP : https://github.com/upstash/context7
Excel MCP: https://github.com/haris-musa/excel-mcp-server
```
