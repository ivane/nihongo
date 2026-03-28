# 🇯🇵 日本語単語帳

多邻国日语学习的单词本 + 记忆模式

## 功能

- 📖 **单词本** — 搜索、分类、卡片/表格两种视图
- 🧠 **记忆模式** — 单词跟读 + 例句跟读，语音识别判对错
- 🔊 **朗读** — TTS 语音朗读，支持浏览器原生 / Azure TTS
- 🗂️ **分类** — 日期、数字、交通、旅游必懂、食物、日常等
- 🔗 **关联词** — 近义词对比，说明使用场景区别
- 🔤 **五十音** — 清音+浊音+拗音，融入记忆模式

## TTS 语音设置

### 引擎选择

点击右上角 🔊 按钮进入 TTS 设置：

| 引擎 | 特点 |
|------|------|
| **本地 TTS** | 免费，无需配置，依赖浏览器自带语音 |
| **Azure TTS** | 高质量神经网络语音，需配置 API Key |

### Azure TTS 配置（可选）

1. 点击 🔊 → 选择 **Azure TTS**
2. 填写 Azure API Key 和 Region（如 `eastus`）
3. 选择语音（男声/女声）
4. 语速和音调可实时调节

**获取 Azure API Key：**
- [Azure Portal](https://portal.azure.com/) → 创建 Speech 资源 → 密钥和终结点
- 每月 50 万字符免费额度

### 语音列表

| 语音 | 特点 |
|------|------|
| Keita | 日语男声（年轻） |
| Daichi | 日语男声（成熟） |
| Mayu | 日语女声 |
| Nanami | 日语女声 |
| Aoi | 日语女声 |

## 技术

- 纯前端，无需后端
- 数据存储在 `words.json`（需手动编辑或通过 + 前缀触发记录）
- GitHub Pages 部署：https://ivane.github.io/nihongo/

## 本地运行

```bash
cd ~/nihongo
# 直接打开 index.html，或启动本地服务器：
python3 -m http.server 8000
# 然后访问 http://localhost:8000
```
