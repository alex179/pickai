# PickAI - Vercel 部署指南

## 🚀 快速部署到 Vercel

### 方式 1: 通过 GitHub 自动部署（推荐）

1. **连接 GitHub**
   - 访问 https://vercel.com
   - 点击 "Import Project"
   - 选择 GitHub 仓库：`alex179/pickai`

2. **配置项目**
   - Framework Preset: **Next.js**
   - Root Directory: `./`
   - Build Command: `npm run build`
   - Output Directory: `.next`

3. **点击 Deploy**
   - Vercel 会自动检测配置
   - 构建完成后获得域名：`https://pickai-xxx.vercel.app`

---

### 方式 2: 通过 Vercel CLI

```bash
# 安装 Vercel CLI
npm i -g vercel

# 登录
vercel login

# 部署
cd ~/workspace/pickai
vercel

# 生产环境部署
vercel --prod
```

---

## 📝 环境变量（可选）

未来需要配置的环境变量：

| 名称 | 值 | 说明 |
|------|-----|------|
| `OPENAI_API_KEY` | sk-xxx | OpenAI API Key |
| `DATABASE_URL` | postgres://xxx | Supabase 数据库 |

---

## ✅ 部署检查清单

- [x] Next.js 配置正确
- [x] package.json 包含 build 脚本
- [x] vercel.json 配置完成
- [x] 代码已推送到 GitHub
- [ ] 连接 Vercel 到 GitHub
- [ ] 首次部署成功

---

**准备好部署了！访问 https://vercel.com 开始吧！** 🚀