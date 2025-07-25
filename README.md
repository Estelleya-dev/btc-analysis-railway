# 🚀 BTC专业分析平台

## 📋 项目概述

专业级BTC分析平台，集成实时价格监控、AI智能分析、新闻监控等功能，为机构投资者提供专业的投资决策支持。

## ✨ 核心功能

- 📈 **实时价格监控** - OKX API集成，多重备用源
- 🤖 **AI智能分析** - DeepSeek深度市场分析  
- 📰 **新闻监控** - 金十数据整合，关键词筛选
- 🔐 **安全认证** - 授权码验证（BTC2025）
- 📱 **响应式设计** - 完美适配各种设备

## 🚀 Railway快速部署

### 方法1：从GitHub部署（推荐）

1. **上传到GitHub**
   ```bash
   # 创建新仓库
   # 上传所有文件到仓库根目录
   ```

2. **连接Railway**
   - 访问 [Railway.app](https://railway.app)
   - 点击 "New Project" → "Deploy from GitHub repo"
   - 选择您的仓库
   - 点击 "Deploy"

3. **配置环境变量**
   在Railway项目的Variables页面添加：
   ```
   DEEPSEEK_API_KEY = 您的DeepSeek API密钥
   OKX_API_KEY = 您的OKX API密钥
   ```

4. **访问应用**
   - 部署完成后获得URL：`https://您的项目名.railway.app`
   - 使用授权码：`BTC2025`

### 方法2：本地开发

1. **安装依赖**
   ```bash
   pip install -r requirements.txt
   ```

2. **设置环境变量**
   ```bash
   export DEEPSEEK_API_KEY="您的API密钥"
   export OKX_API_KEY="您的API密钥"
   ```

3. **运行应用**
   ```bash
   python app.py
   ```

## 📁 文件结构

```
btc-analysis-platform/
├── app.py              # Flask主应用
├── requirements.txt    # Python依赖
├── Procfile           # Railway启动配置
├── railway.toml       # Railway项目配置
├── runtime.txt        # Python版本
├── .gitignore         # Git忽略文件
└── README.md          # 项目说明
```

## 🔧 技术架构

- **后端框架**: Flask + Gunicorn
- **API集成**: OKX、DeepSeek、CoinGecko
- **部署平台**: Railway
- **前端技术**: HTML5 + CSS3 + JavaScript

## 🔐 安全特性

- 授权码验证系统
- API密钥环境变量管理
- HTTPS加密传输
- 错误处理和重试机制

## 📊 API接口

- `GET /` - 主页面
- `GET /api/price` - 获取BTC价格
- `POST /api/analysis` - AI分析
- `GET /api/news` - 新闻数据
- `GET /api/status` - 系统状态
- `GET /health` - 健康检查

## 🚨 故障排除

1. **部署失败**
   - 检查requirements.txt依赖
   - 确认Python版本兼容性

2. **API调用失败**
   - 检查环境变量配置
   - 验证API密钥有效性

3. **页面无法访问**
   - 检查Railway部署状态
   - 查看部署日志错误信息

## 📞 支持

如有问题，请检查：
1. Railway部署日志
2. 环境变量配置
3. API密钥权限
---

⚡ **授权码**: BTC2025  
🔗 **部署平台**: Railway.app  
💡 **适用场景**: 机构投资、专业分析、实时监控
