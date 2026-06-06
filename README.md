# 💾 Backup Tools

AI备份工具，支持备份策略生成、脚本生成、恢复计划。

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-blue?logo=python" />
  <img src="https://img.shields.io/badge/OpenAI-API-green?logo=openai" />
  <img src="https://img.shields.io/badge/License-MIT-yellow" />
</p>

## ✨ 特性

- 📋 备份策略生成
- 📝 备份脚本生成
- 🔄 恢复计划生成
- 🧪 备份测试方案
- 💾 存储需求估算

## 🚀 快速开始

```bash
pip install openai

python tools.py
```

## 📖 使用

```python
from backup_tools import create_tools

tools = create_tools()

# 生成策略
strategy = tools.generate_strategy("数据库", "100GB", "high")

# 生成备份脚本
script = tools.generate_backup_script("/data", "/backup", "rsync")

# 生成恢复计划
plan = tools.generate_recovery_plan("硬件故障", ["数据库", "文件服务器"])

# 测试方案
test = tools.test_backup("/backup/full_20240115.tar.gz")

# 估算存储
estimate = tools.estimate_storage("500GB", 30)
```

## 📁 项目结构

```
backup-tools/
├── tools.py       # 备份工具核心
└── README.md
```

## 📄 许可证

MIT License
