# agent-harness-go
使用 Go 语言构建 AI Agent Harness

## 01
```bash
go mod init github.com/bingohuang/agent-harness-go
```

```bash
mkdir -p cmd/claw
mkdir -p internal/engine     # 核心引擎层 (Main Loop)
mkdir -p internal/provider   # 模型适配层 (Claude/Zhipu Adapter)
mkdir -p internal/context    # 上下文工程层 (Compactor, Prompt Composer)
mkdir -p internal/tools      # 工具与执行层 (Registry, Built-in Tools)
mkdir -p internal/memory     # 状态与记忆层 (基于文件的 PLAN/TODO)
mkdir -p internal/feishu     # 飞书集成层
```

```bash
mkdir -p cmd/claw internal/{engine,provider,context,tools,memory,feishu}
```


## 04
```bash
go get github.com/openai/openai-go/v3
go get github.com/anthropics/anthropic-sdk-go
```