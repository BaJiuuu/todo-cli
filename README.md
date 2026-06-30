[README.md](https://github.com/user-attachments/files/29507190/README.md)
# 📝 Todo CLI

一个用 Python 实现的简洁命令行待办事项管理工具。

## 功能特性

- ✅ 添加待办事项
- 📋 查看待办列表
- 🎉 标记任务完成
- 🗑️ 删除任务
- 🔍 搜索任务
- 💾 SQLite 本地存储，数据持久化

## 环境要求

- Python 3.6+
- 无需安装额外依赖（使用 Python 标准库）

## 使用方法

```bash
# 添加任务
python todo.py add "学习Python基础语法"
python todo.py add "完成数据结构作业"

# 查看待办任务
python todo.py list

# 查看所有任务（包括已完成）
python todo.py list --all

# 标记任务完成（根据ID）
python todo.py done 1

# 删除任务
python todo.py delete 1

# 搜索任务
python todo.py search "Python"

# 查看帮助
python todo.py help
```

## 运行效果

```
$ python todo.py add "学习Python"
✅ 已添加: 学习Python

$ python todo.py add "刷LeetCode"
✅ 已添加: 刷LeetCode

$ python todo.py list

==================================================
  ID    状态    内容                          创建时间
==================================================
  1     ⏳    学习Python                    2025-07-01 10:30
  2     ⏳    刷LeetCode                    2025-07-01 10:31
==================================================
  共 2 项 | 待完成: 2 | 已完成: 0

$ python todo.py done 1
🎉 已完成: 学习Python
```

## 项目结构

```
todo-cli/
├── todo.py        # 主程序
├── README.md      # 项目说明
└── todos.db       # SQLite 数据库文件（运行后自动生成）
```

## 技术要点

- Python 基础语法（函数、条件、循环）
- SQLite 数据库操作
- 命令行参数解析
- 异常处理

## 作者

你的名字 - [GitHub](https://github.com/你的用户名)
