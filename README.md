# AI 文案生成器

基于智谱 AI（GLM-4.6V）的多模态文案生成工具，支持图片识别生成文案和文字描述生成文案两种模式。

## 功能

- **图片生成文案**：上传产品图片，AI 识别图片内容并生成营销文案
- **文字生成文案**：输入产品描述，AI 根据描述生成多风格文案

## 技术栈

- 前端：HTML + CSS + JavaScript
- 后端：Python Flask
- AI：智谱 GLM-4.6V（图片+文案）/ GLM-4 Flash（纯文字）

## 快速开始

### 1. 安装依赖

```bash
pip install -r requirements.txt
```

### 2. 配置 API Key

复制 `.env.example` 为 `.env`，填入你的智谱 API Key：

```bash
cp .env.example .env
```

然后编辑 `.env` 文件，将 `your_api_key_here` 替换为你的真实 API Key。

> 去 https://bigmodel.cn 注册获取 API Key。

### 3. 启动后端

```bash
python backend.py
```

后端启动后运行在 http://localhost:5000

### 4. 打开前端

用浏览器打开 `index.html` 即可使用。

## 项目结构

```
ai-copywriter/
├── index.html        # 前端页面
├── backend.py        # Flask 后端服务
├── requirements.txt  # Python 依赖
├── .env.example      # 环境变量模板
└── .gitignore        # Git 忽略规则
```