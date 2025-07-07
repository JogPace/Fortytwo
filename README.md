
# Fortytwo节点运营

Fortytwo是monad生态项目，运营节点需要GPU和节点激活码，在这里申请:https://tally.so/r/wQzVQk

---
# Fortytwo 节点安装教程（适用于 Linux）
---

## ✨ 前置要求

* 一台 Ubuntu VPS（推荐 22.04 或 24.04），需要有GPU,显存不低于6G.
* 安装了 `curl`、`unzip` 和 `screen`
* 有 Fortytwo 邀请码

如未安装依赖，请执行：

```bash
sudo apt update && sudo apt install -y curl unzip screen
```

---

## 🚀 安装步骤

1. **创建项目目录并进入**

```bash
mkdir -p ~/Fortytwo && cd ~/Fortytwo
```

2. **下载 Fortytwo**

```bash
curl -L -o fortytwo-console-app.zip https://github.com/Fortytwo-Network/fortytwo-console-app/archive/refs/heads/main.zip
```

3. **解压并进入目录**

```bash
unzip fortytwo-console-app.zip
cd fortytwo-console-app-main
```

4. **运行安装脚本**
---

```bash
screen -S fortytwo
chmod +x linux.sh
./linux.sh

---

## 启动节点（根据提示完成）

安装完成后，根据提示，输入1，系统会提示你输入 **激活码**。激活码必须事先通过官网申请：

👉 [申请邀请码](https://tally.so/r/wQzVQk)

---

## 选择模型

可以根据自己显存大小选择模型，正常运行后，按：Ctrl+A+D 退出screen会话。

## 🛠 管理节点

使用 `screen` 可以查看或重连运行中的控制台：

* 查看当前 screen 会话：

```bash
screen -ls
```

* 连接已有会话（假设名为 fortytwo）：

```bash
screen -r fortytwo
```

* 退出 screen 不关闭程序：按下 `Ctrl+A` 后松开再按 `D`。

---

