# 🚀 iRolixBot

<div align="center">

<img src="https://raw.githubusercontent.com/iitzSeriZdev/iRolixBot/main/iRolix%20Logo.png" alt="iRolix Logo" style="background: white; padding: 20px; border-radius: 12px; max-width: 300px;">

| [![版本](https://img.shields.io/badge/版本-1.0.0-blue.svg)](https://github.com/iitzSeriZdev/iRolixBot) [![许可证](https://img.shields.io/badge/许可证-MIT-green.svg)](LICENSE) [![PHP](https://img.shields.io/badge/PHP-8.2%2B-7777BB?logo=php)](https://php.net) ⚡ **高级 Telegram VPN 销售机器人，带管理面板**

**VPN 服务提供商的终极解决方案**

使用功能强大的 Telegram 机器人转变您的 VPN 业务，该机器人可自动化销售、管理用户并简化您的运营。

[English](README.md) • [فارسی](README.fa.md) • [中文](#) • [Русский](README.ru.md)

[🌟 星标](https://github.com/iitzSeriZdev/iRolixBot) • [🐛 报告错误](https://t.me/iRolix_Bot/8) • [💡 请求功能](https://t.me/iRolix_Bot/10) • [📖 文档](#-文档)

</div>

---

## 📋 目录

- [✨ 功能](#-功能)
- [🎯 主要亮点](#-主要亮点)
- [📦 要求](#-要求)
- [🚀 快速开始](#-快速开始)
- [⚙️ 配置](#️-配置)
- [🌐 VPN 面板支持](#-vpn-面板支持)
- [💳 支付网关](#-支付网关)
- [🔒 安全性](#-安全性)
- [📚 文档](#-文档)
- [💬 支持与社区](#-支持与社区)
- [💰 支持开发](#-支持开发)
- [📄 许可证](#-许可证)

---

## ✨ 功能

### 🤖 机器人功能

- **📱 订阅管理**
  - 购买订阅（类型、流量、时长）
  - 服务续费和延期
  - 购买额外流量和天数
  - 测试服务（一次性）
  - 服务信息和详情

- **👥 用户管理**
  - 用户账户信息
  - 交易历史
  - 推荐统计
  - 余额管理

- **💳 支付系统**
  - 多个支付网关（Zarinpal、卡对卡等）
  - 自动支付处理
  - 发票管理
  - 支付验证

- **🎁 推荐计划**
  - 独特的推荐链接
  - 可自定义佣金（百分比/固定）
  - 自动支付
  - 推荐统计

- **🎫 支持系统**
  - 基于工单的支持
  - 管理员通知
  - 消息转发

### 👨‍💼 管理员功能

- **📊 机器人内管理面板**
  - 用户管理
  - 服务管理
  - 产品管理
  - 面板管理
  - 日志和统计
  - 设置配置

- **🌐 Web 管理面板**
  - 完整的统计仪表板
  - 用户管理界面
  - 服务管理
  - 产品管理
  - VPN 面板管理
  - 发票管理
  - 推荐系统管理
  - 安全监控
  - 综合日志记录
  - 多语言支持（英语、波斯语、中文、俄语）

### 🔒 安全功能

- **🛡️ 反垃圾邮件系统**
  - 可配置的点击率限制
  - 自动静音功能
  - 基于时间的限制

- **🚨 反欺诈系统**
  - 管理员活动监控
  - 自动撤销访问
  - 可疑活动检测

- **📊 安全监控**
  - IP 跟踪
  - 浏览器和操作系统检测
  - 国家检测
  - 活动记录

- **🔐 附加安全**
  - Telegram IP 验证
  - SQL 注入防护
  - XSS 防护
  - CSRF 防护
  - 速率限制
  - 安全会话管理

---

## 🎯 主要亮点

- ✅ **多语言支持** - 完全支持英语、波斯语、中文和俄语
- ✅ **双机器人架构** - PHP 机器人用于共享主机，Python 机器人用于 VPS
- ✅ **多个 VPN 面板** - 支持 12+ 种 VPN 面板类型
- ✅ **支付网关** - 与伊朗和国际支付网关集成
- ✅ **自动化安装** - 两种主机类型的一键安装
- ✅ **专业管理面板** - 具有现代 UI 的基于 Web 的管理面板
- ✅ **高级安全性** - 反垃圾邮件、反欺诈和综合监控
- ✅ **推荐系统** - 完整的推荐和联盟计划
- ✅ **QR 码生成** - 带背景图像的自定义 QR 码

---

## 📦 要求

### 服务器要求

**对于 PHP 机器人（共享主机）：**
- PHP >= 8.1
- MySQL/MariaDB >= 5.7
- 带 mod_rewrite 的 Apache/Nginx
- cURL 扩展
- PDO MySQL 扩展
- mbstring 扩展
- GD 扩展（用于 QR 码）
- BCMath 扩展
- 日志和上传的写入权限

**对于 Python 机器人（VPS）：**
- Python 3.9+
- MySQL/MariaDB >= 5.7
- Nginx（推荐）
- Systemd（用于服务管理）

### PHP 扩展

- `pdo_mysql` - 数据库连接
- `curl` - HTTP 请求
- `json` - JSON 处理
- `mbstring` - 多字节字符串处理
- `gd` - 图像处理（QR 码）
- `bcmath` - 数学运算

### PHP 库（Composer）

- `endroid/qr-code` ^4.0 - QR 码生成
- `guzzlehttp/guzzle` ^7.0 - HTTP 客户端

---

## 🚀 快速开始

### 📦 自动化安装（推荐）

#### 对于共享主机

1. 将所有项目文件上传到您的主机
2. 导航到：`https://yourdomain.com/installer/host/install.php`
3. 按照安装向导操作：
   - 步骤 1：检查要求
   - 步骤 2：配置数据库
   - 步骤 3：配置机器人
   - 步骤 4：自动安装
   - 步骤 5：完成！

#### 对于 VPS（Ubuntu/Debian）

```bash
# 一键安装
sudo bash <(curl -sSL https://raw.githubusercontent.com/iitzSeriZdev/iRolixBot/main/installer/vps/install.sh) install

# 带备份卸载
sudo bash <(curl -sSL https://raw.githubusercontent.com/iitzSeriZdev/iRolixBot/main/installer/vps/install.sh) uninstall-with-backup

# 直接更新
sudo bash <(curl -sSL https://raw.githubusercontent.com/iitzSeriZdev/iRolixBot/main/installer/vps/install.sh) update
```

**安装后：**

1. 数据库凭据保存到 `/tmp/irolix_db_config`
2. 编辑 `/opt/iRolixBot/bot-php/config.php` 以添加您的机器人令牌
3. 在 `http://YOUR_SERVER_IP/web-panel` 访问面板
4. 通过 Web 界面完成设置

### 📦 手动安装

如果您更喜欢手动安装：

#### 步骤 1：克隆存储库

```bash
git clone https://github.com/iitzSeriZdev/iRolixBot.git
cd iRolixBot
```

#### 步骤 2：安装依赖项

```bash
cd bot-php
composer install
```

#### 步骤 3：设置数据库

创建 MySQL/MariaDB 数据库并记录凭据。

#### 步骤 4：创建 Telegram 机器人

1. 在 Telegram 上向 @BotFather 发送消息
2. 使用 `/newbot` 创建您的机器人
3. 安全保存机器人令牌

#### 步骤 5：运行安装

1. 将文件上传到您的 Web 服务器
2. 在浏览器中访问 `installer/host/install.php`
3. 按照直观的安装向导操作：
   - 选择您的语言
   - 输入数据库详细信息
   - 配置机器人令牌
   - 设置管理员账户
   - 完成安装

#### 步骤 6：设置 Cron Jobs

配置**仅一个 cron job**：

```bash
* * * * * /usr/bin/php /path/to/iRolixBot/bot-php/cron/cron.php >> /path/to/iRolixBot/Logs/cron_output.log 2>&1
```

或使用 HTTP：

```bash
* * * * * curl -s https://yourdomain.com/bot-php/cron/cron.php > /dev/null 2>&1
```

**就是这样！** 集中管理器自动处理所有内容。🎉

---

## ⚙️ 配置

安装后，自定义您的机器人：

1. **🔌 VPN 面板** - 连接您的面板
2. **💳 支付网关** - 设置支付方式
3. **⚙️ 机器人设置** - 自定义行为
4. **👥 用户** - 管理客户
5. **🛍️ 产品** - 创建产品
6. **📁 类别** - 组织产品

---

## ⏰ Cron Jobs

### 自动执行什么？

- **每分钟** ⚡ - 支付、通知、消息
- **每 2 分钟** 🎁 - 礼品系统、配置测试
- **每 3 分钟** 💰 - 支付网关检查
- **每 5 分钟** 📊 - 支付过期、报告
- **每 15 分钟** 🔍 - 状态检查、监控
- **每 30 分钟** ⏳ - 代理过期
- **每小时** 🎲 - 抽奖系统
- **每 5 小时** 💾 - 自动备份

---

## 🌐 VPN 面板支持

### OpexCore 库面板：
- ✅ **Marzban** - 现代 V2Ray/Xray 面板
- ✅ **Marzneshin** - 高级 VPN 面板
- ✅ **ovPanel** - OpenVPN 面板
- ✅ **Pasarguard** - 安全 VPN 面板
- ✅ **Remnawave** - Wave VPN 面板
- ✅ **Guard Panel** - 专注于安全的面板

### 基于 PHP 的面板：
- ✅ **Ali Reza** - 流行的伊朗面板
- ✅ **Ali Reza Single Port** - 单端口变体
- ✅ **3x-ui** - Xray UI 面板
- ✅ **x-ui Single Port** - 单端口 Xray UI
- ✅ **S-ui** - 简单 UI 面板
- ✅ **Mikrotik** - RouterOS 集成
- ✅ **WGDashboard** - WireGuard 仪表板
- ✅ **Hiddify** - Hiddify 面板
- ✅ **Sanaei** - Sanaei 面板

---

## 💳 支付网关

### 伊朗网关：
- ✅ **Zarinpal** - 最受欢迎的伊朗网关
- ✅ **Nowpayment** - 现代支付网关
- ✅ **IranPay1** - 伊朗支付网关
- ✅ **Aqayepardakht** - 支付网关
- ✅ **卡对卡** - 直接卡转账

### 国际网关：
- ✅ **Yoomoney** - 俄罗斯支付系统
- ✅ **Yookassa** - Yandex 支付网关
- ✅ **Freekassa** - 国际网关
- ✅ **Heleket** - 支付网关
- ✅ **Robokassa** - 俄罗斯支付网关
- ✅ **Telegram Stars** - Telegram 的支付系统
- ✅ **Cryptomus** - 加密货币网关
- ✅ **CryptoPay** - 加密支付网关

---

## 🔒 安全性

### 安全功能

- ✅ Telegram IP 验证
- ✅ SQL 注入防护（预处理语句）
- ✅ XSS 防护
- ✅ CSRF 防护
- ✅ 速率限制
- ✅ 安全会话管理
- ✅ 反垃圾邮件系统
- ✅ 反欺诈系统
- ✅ 安全监控

### 安全最佳实践

1. **安装后：**
   - 删除 `installer` 目录
   - 更改默认密码
   - 设置 SSL/TLS 证书

2. **定期维护：**
   - 定期更新依赖项
   - 定期查看日志
   - 定期备份数据库

3. **服务器安全：**
   - 使用强密码
   - 启用防火墙
   - 保持系统更新

有关详细的安全信息，请参阅 [SECURITY.md](SECURITY.md)

---

## 📚 文档

- 📖 [安装指南](HOST_INSTALLATION_GUIDE.md)
- 🔒 [安全指南](SECURITY.md)
- ⏰ [Cron 设置](CRON_SETUP.md)
- 📊 [项目摘要](PROJECT_SUMMARY_FOR_HOST.md)

---

## 💬 支持与社区

### 获取帮助

- 💬 **Telegram 群组**: [@iRolix_Bot](https://t.me/iRolix_Bot) - 加入我们的社区！
- 🐛 **错误报告**: [报告问题](https://t.me/iRolix_Bot/8) - 帮助我们改进！
- 💡 **建议**: [分享想法](https://t.me/iRolix_Bot/10) - 您的想法很重要！

### 关注开发者

- 🐙 **GitHub**: [@iitzSeriZdev](https://github.com/iitzSeriZdev)
- 🎥 **YouTube**: [@iitzSeriZ](https://youtube.com/@iitzSeriZ)
- 🐦 **X (Twitter)**: [@iitzSeriZ](https://x.com/iitzSeriZ)

---

## 💰 支持开发

### 🌟 帮助我们建设未来！🌟

**您的支持在世界上产生巨大影响！**

我们致力于使 iRolixBot 成为可用的最佳 Telegram 机器人解决方案。您的捐赠直接推动更快的开发、独家功能和持续改进。

### 🚀 为什么您的捐赠很重要

您慷慨的捐赠使我们能够：

- ⚡ **加速开发** - 更多捐赠 = 更快的功能发布和更新
- 🎯 **构建独家功能** - 获得前沿功能
- 🛠️ **增强支持** - 为我们慷慨的捐赠者提供优先支持
- 🌟 **持续创新** - 保持项目活跃、蓬勃发展并不断演进
- 🔒 **更好的安全性** - 投资安全审计和改进
- 📚 **综合文档** - 创建更好的指南和教程

### 💎 您给予的越多，得到的越多！

**每次捐赠都让我们更接近目标！**

- **更高的捐赠** = **优先访问**新功能
- **更快的更新** = **更频繁的发布**，包含错误修复和改进
- **独家功能** = **独特功能**，使 iRolixBot 与众不同
- **更好的支持** = **更快的响应时间**和专门协助

### 💳 如何捐赠

选择您首选的支付方式：

#### 💰 加密货币（直接转账）

| 货币      | 网络                        | 地址                                           |
| --------- | --------------------------- | ---------------------------------------------- |
| 💵 **USDT** | BEP20 (Binance Smart Chain) | 0xCaF05b21A518E6750AA43aD87cEB4a725e78a850     |
| 💎 **TON**  | The Open Network            | UQAg7NaXzzFMvGxqirO9UYwwzseq8pAi3N8fompkKjOFtIzl |
| 💰 **TRX**  | Tron Network                | TPatJCKdLJs1ZpetLtpC97nsHg8X9G1KRs             |

> ⚠️ **重要提示：** 发送加密货币时，请确保使用正确的网络！

#### 💸 在线支付（推荐）

**🌐 通过 NowPayments 捐赠**

NowPayments 接受：
- 💳 信用卡/借记卡
- 💰 100+ 加密货币
- 🌍 多种支付方式
- 🔒 安全快速处理

**无论金额大小，每次捐赠都有助于我们改进 iRolixBot 并为您带来更好的功能！** 🙏

---

## 📄 许可证

本项目根据 **MIT 许可证** 许可 - 详细信息请参阅 [LICENSE](LICENSE) 文件。

您可以自由使用、修改和分发本项目！🎉

---

<div align="center">

### 由 iitzSeriZ 用 💜 制作

**如果您觉得此存储库有用，请考虑给它一个星标！** ⭐

⭐ [星标](https://github.com/iitzSeriZdev/iRolixBot) • 🐛 [报告错误](https://t.me/iRolix_Bot/8) • 💡 [请求功能](https://t.me/iRolix_Bot/10) • 💸 [捐赠](#-支持开发)

**#woman_life_freedom**

</div>

