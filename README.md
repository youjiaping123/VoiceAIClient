# VoiceAI客户端部署指南

## 项目简介

VoiceAI是一个基于MQTT协议的语音AI助手，集成了OpenAI的AI模型和Azure的语音服务，实现了语音对话功能。

## 快速开始


#### 1. 克隆代码

```bash
git clone https://github.com/youjiaping123/VoiceAIClient
cd VoiceAIClient
```

#### 2.2 配置环境变量

创建并编辑 .env 文件：

```bash
vi .env
```

配置以下环境变量：

```
MQTT_BROKER=你的服务器IP
MQTT_PORT=1883
```

#### 3.3 创建并激活Python虚拟环境

```bash
python3 -m venv venv
source venv/bin/activate
```

#### 3.4 安装依赖

```bash
pip install -r requirements.txt
```

#### 3.5 启动服务

```bash
python Client.py
```

## 配置说明

- MQTT_BROKER：MQTT服务器地址
- MQTT_PORT：MQTT服务端口默认为1883

## 常见问题

1. 如遇到连接MQTT服务器失败，请检查防火墙设置
2. 确保所有环境变量都已正确配置

## 许可证

[MIT License](LICENSE)