# 💪 健身饮食打卡 Fitness Tracker

一个简单好用的健身 + 饮食打卡 Web App：30 分钟无氧 + 30 分钟有氧的训练节奏、按拳头目测的饮食记录、自动计算的热量目标和渐进超负荷建议。专为忙碌的上班族设计——每天打卡只需要 1 分钟。

A lightweight workout & diet check-in PWA: strength + cardio tracking, fist-sized portion logging, personalized calorie targets, and progressive-overload suggestions. Built for busy people — daily check-in takes under a minute.

**👉 立即使用 Use it now: https://maggie-cl.github.io/fitness-app/**

---

## 📲 安装 Install (iPhone)

1. 用 **Safari** 打开上面的链接
2. 点击分享按钮 (□↑) → **添加到主屏幕 Add to Home Screen**
3. 完成！像原生 app 一样全屏运行，支持离线使用

Android: Chrome 打开链接 → 菜单 → 添加到主屏幕。

## 🚀 快速开始 Quick Start

1. **填资料**：打开 设置 Settings → 填写昵称、身高、体重、目标体重、年龄、性别、活动量 → 保存。热量和蛋白质目标会自动按你的情况计算（Mifflin-St Jeor 公式，每日约 500 kcal 缺口）
2. **定课表**：设置 → 每周课表，每天选择 类型（健身房/居家/休息）+ 无氧部位 + 有氧分钟数
3. **每天打卡**：今日 Today 页从上到下——无氧 ✓ → 有氧 ✓ → 三餐 ✓ → 喝水 → 体重
4. **看进度**：体重 Weight 页看趋势线，历史 History 页看连续打卡和周报

## ✨ 功能 Features

### ✅ 今日打卡 Today
- **无氧训练**：每天按课表自动生成动作清单，每个动作记录 重量 × 次数 × 组数
  - 🧠 **渐进超负荷自动建议**：上次做满 12 次 → 自动建议加重；没满 → 建议 +1 次。数值已预填，按计划完成直接点 ✓
  - 📌 **动作记忆**：换过/增删的动作会被记住，同部位下次训练默认沿用你上次打卡的动作清单
  - 🔄 **智能替换**：删除动作时推荐同肌群的护膝替代动作
  - ⏱ **组间休息计时器**：60s / 90s 倒计时，结束提示音
- **有氧打卡**：快走/爬坡/爬楼机/椭圆机/HIIT/健身操等，可自定义添加；记录时长
- **饮食打卡**：早/午/晚三餐 + 可选加餐
  - 蛋白质种类多选（三文鱼/鸡肉/牛肉/豆腐/鸡蛋/牛奶/蛋白粉）
  - 用 **拳头** 目测份量（1拳 ≈ 100g），建议值已按你的目标预填
  - 每餐显示估算热量；加餐从固定份量的食物列表一键选择
- **🔥 热量平衡**：摄入 vs 消耗（基础代谢 + 力量 + 有氧，按 MET 公式估算）vs 缺口，400~700 kcal 缺口显示 ✓
- **💧 饮水**：点杯子记录，一杯 0.8L，目标 3L
- **⚖️ 体重·腰围**：体重每天记，腰围每周记

### 📉 体重 Weight
- 体重趋势图：每日数据点 + 7 日均线 + 目标线
- 腰围趋势图（减脂增肌期腰围比体重更诚实）

### 📅 历史 History
- 打卡日历：绿色=全完成，黄色=部分完成；点任意过去日期可补打卡
- 🔥 连续打卡天数（streak）
- 周报：无氧次数 / 有氧次数 / 周均体重变化 / 蛋白质达标天数 / 饮水达标天数

### ⚙️ 设置 Settings
- **个人资料**：所有目标（热量/蛋白质/碳水/每餐份量/起始重量）按 年龄/性别/身高/体重/目标体重/活动量 自动个性化
- **每周课表**：每天自由配置——类型、无氧部位（下肢臀腿/上肢/全身/核心/居家哑铃/低冲击循环 预设）、有氧分钟数；选休息日自动清空当天安排
- **数据备份**：一键导出/导入 JSON

## 🦵 护膝设计 Knee-Friendly by Default

默认课表避开伤膝动作（深蹲、箭步蹲、跳绳、登山跑等），以髋主导动作为主（罗马尼亚硬拉、臀推、腿弯举、高箱浅蹲）；有氧默认低冲击（快走/椭圆机/单车）。膝盖好的用户可以在课表里自由替换动作。

## 🔒 数据与隐私 Data & Privacy

- **所有数据只存在你的设备上**（浏览器 localStorage），不上传任何服务器
- 更新 app 不影响已有数据；建议每周用 设置 → 导出备份 保存一份 JSON
- 删除主屏幕图标或清除浏览器数据会丢失记录——先导出！
- 多人使用同一链接互不影响，每台设备独立

## 🛠 技术 Tech

- 单文件 HTML + 原生 JavaScript + SVG 图表，零依赖
- PWA（manifest + service worker），支持离线使用
- 托管于 GitHub Pages

本地运行：`python3 -m http.server 8000` 然后打开 `http://localhost:8000`。

## ⚠️ 免责声明 Disclaimer

本应用的饮食与训练建议仅供参考，不构成医疗建议。开始任何减重或训练计划前，请咨询医生——尤其是孕产期、哺乳期或有慢性疾病的用户。

The diet and training suggestions in this app are for reference only and do not constitute medical advice. Consult your physician before starting any weight-loss or training program.

---

🤖 Built with [Claude Code](https://claude.com/claude-code)
