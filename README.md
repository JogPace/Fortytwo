
## Fortytwo节点

运营 Fortytwo 节点，其实就是把你设备的算力贡献出来，帮忙跑一些小模型，参与处理 AI 推理任务，按你提供的资源多少，拿到积分奖励。

这个项目比较人性的化的是，只有申请到激活码，运行节点需要的GAS（mon）项目方会每天打到你的钱包。

### Fortytwo 节点安装教程（适用于 Linux）

---

#### ✨ 前置要求

* 一台 Ubuntu VPS（推荐 22.04 或 24.04），8核16G，硬盘20G，需要有GPU,显存不低于6G.
* 安装了 `curl`、`unzip` 和 `screen`
* 有 Fortytwo 邀请码，没有在这里申请:https://tally.so/r/wQzVQk

如未安装依赖，请执行：

```bash
sudo apt update && sudo apt install -y curl unzip screen
```
---

#### 安装步骤

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

```bash
screen -S fortytwo
chmod +x linux.sh
./linux.sh
```
---

#### 启动节点（根据提示完成）

安装完成后，根据提示，输入1，系统会提示你输入 **激活码**。激活码必须事先通过官网申请：

👉 [申请邀请码](https://tally.so/r/wQzVQk)

首次运行会生成助记词等账户信息，请根据提示保存。

把助记词导入钱包，可以看到账户余额，如果正常运行，账户42T会一直增加：

42T ca: 0x22A3d96424Df6f04d02477cB5ba571BBf615F47E

![image](https://github.com/user-attachments/assets/3ad7a2d9-4307-479e-87b0-47a909f1e404)

---

#### 选择模型

可以根据自己显存大小选择模型，正常运行后，按：Ctrl+A+D 退出screen会话。

![image](https://github.com/user-attachments/assets/5325ced1-8075-4208-bbed-fa233ad2de44)

---

####  管理节点

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



