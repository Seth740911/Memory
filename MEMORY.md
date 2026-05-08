# 长期记忆

## 用户信息
- **姓名**：时帅（老时）
- **职业**：前端开发，自称小白，Git与命令行经验少
- **偏好**：简单直接，厌恶复杂步骤和过度解释，让AI直接执行而非给手动步骤
- **关注**：AI coding和具身智能领域最新动态

## 项目信息

### 中标啦（SV）

#### 电脑标识
- **家中笔记本**：NOTEBOOK-SETH（主机名），项目目录 `G:\SV\`
- **单位电脑**：（待确认主机名），项目目录 `D:\SETH\SV\`
- Windows 用户名：`Administrator`

#### 项目路径
- 单位电脑：`D:\SETH\SV\`
- 家中电脑：`G:\SV\`（有时也用 `G:\AI\SV\`）
- 云端地址：https://ai-native-d3g2ds7183df62e2b-1323153036.tcloudbaseapp.com
- GitHub：https://github.com/Seth740911/SV
- 技术栈：React 18 + TypeScript + Ant Design 5 + Vite + CloudBase
- 本地开发端口：http://localhost:3004

#### 供应商管理模块（2026-05-06 完成）
- 主入口：`src/renderer/pages/SuppliersPage.tsx`
- 5个Tab组件：
  - `SupplierBasicTab.tsx` - 基本信息
  - `SupplierContractTab.tsx` - 合同管理
  - `SupplierProgressTab.tsx` - 进度管理
  - `SupplierResponseTab.tsx` - 响应管理
  - `SupplierPaymentTab.tsx` - 付款管理
- 云函数：`cloudfunctions/suppliers/index.js`（通用CRUD）
- 新增集合：supplier_contracts、supplier_progress、supplier_responses、supplier_payments

### 时时张罗（LY）

#### 项目路径
- `G:\AI\LY\`（2026-05-07 从 `C:\Users\Administrator\CodeBuddy\20260420085217\` 迁移）

#### 技术栈
- 微信小程序，微信云开发（Skyline 渲染引擎）
- 云端环境：`cloud1-d4g22qlv474c85bf3`
- AppID：`wx0b14f79dcaf26f7f`

#### 核心功能
- 五个 Tab：首页/预订/日程/记账/我的
- 出行人员管理、行李清单、汇率转换
- 基于 `currentOpenid` 的权限模型（organizer/participant/canEditSchedule）

## 部署命令
```bash
cd G:\SV
git add . && git commit -m "描述" && git push origin main
npm run build:renderer
tcb hosting deploy dist -e ai-native-d3g2ds7183df62e2b
```

## 备份记录
- 2026-05-06：家中笔记本完整备份（GitHub + 腾讯云）
- 2026-05-07：时时张罗迁移到 `G:\AI\LY\`，SETH 迁移到 `G:\SV\`

## 记忆同步策略
- **GitHub 仓库**：Seth740911/Memory（专用记忆仓库）
- **本地路径**：D:\SETH\.workbuddy\memory\（单位）/ G:\SV\.workbuddy\memory\（家中）
- 工作前：`git pull` 拉取最新记忆
- 工作后：`git commit + git push` 上传记忆
- **重要**：两台电脑共用同一个仓库，换电脑后拉取即可同步

## MCP 配置
- MCP server：https://mcp.hermesagent.org.cn/v1（OpenRouter）
