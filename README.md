# 映雪安全工具箱 (YingxueSec-Tools)

跨平台安全工具桌面应用，提供开箱即用的图形化安全工具集。

## 下载安装

前往 [Releases](https://github.com/YingxueSec/YingxueSec-Tools/releases) 下载最新版本：

| 平台 | 文件 | 说明 |
|------|------|------|
| **macOS** | `映雪安全工具箱.app.zip` | 解压后双击运行 |
| **Windows** | `YingxueSec-Toolbox.exe` | 直接双击运行 |

> ⚠️ macOS 首次运行可能提示"无法验证开发者"，请在"系统偏好设置 → 安全性与隐私"中允许运行。

---

## 功能介绍

### 🐕 HTTPDog - 域名存活检测

批量检测域名的 HTTP/HTTPS 存活状态，自动解析 IP 地址。

#### 使用步骤

1. **导入域名**
   - 点击「选择文件」导入 .txt 文件（每行一个域名）
   - 或直接在文本框中粘贴域名列表

2. **开始检测**
   - 点击「开始检测」按钮
   - 等待检测完成，进度条显示当前进度

3. **查看结果**
   - 表格展示：域名、IP、URL、存活状态
   - ✅ 绿色：存活  ❌ 红色：不存活

4. **导出结果**
   - 📋 **复制**：复制所有存活 URL 到剪贴板
   - 📥 **下载 CSV**：导出完整结果到 CSV 文件

#### 示例

输入：
```
baidu.com
qq.com
taobao.com
notexist12345.com
```

输出表格：
| 域名 | IP | URL | 状态 |
|------|-----|-----|------|
| baidu.com | 110.242.68.66 | https://baidu.com | ✅ |
| qq.com | 113.108.81.189 | https://qq.com | ✅ |
| taobao.com | 59.82.122.140 | https://taobao.com | ✅ |
| notexist12345.com | - | - | ❌ |

---

## 常见问题

**Q: macOS 提示"已损坏，无法打开"？**
```bash
xattr -cr /Applications/映雪安全工具箱.app
```

**Q: Windows 提示"Windows 保护了你的电脑"？**  
点击「更多信息」→「仍要运行」

**Q: 检测速度慢？**  
使用内置 itdog 服务检测，速度取决于网络状况，请耐心等待。

---

## 反馈与支持

- 🐛 问题反馈：[GitHub Issues](https://github.com/YingxueSec/YingxueSec-Tools/issues)
- 📧 联系邮箱：security@yingxue.com

---

## 许可证

MIT License
