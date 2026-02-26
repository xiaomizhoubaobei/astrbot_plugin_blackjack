# 21点游戏插件
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fxiaomizhoubaobei%2Fastrbot_plugin_blackjack.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fxiaomizhoubaobei%2Fastrbot_plugin_blackjack?ref=badge_shield)


一个基于AstrBot框架的21点游戏插件，支持PVE和PVP模式，具有完整的赌场级21点规则。

## 功能特性

- ✅ 经典21点游戏规则
- 🎯 PVE模式（玩家对战AI庄家）
- 👥 PVP模式（玩家之间对战）
- 💰 下注系统
- 🔄 支持加倍、分牌、投降、保险等高级玩法
- 📊 个人战绩统计
- 🏆 盈亏排行榜
- 🎮 简单直观的命令交互

## 安装方法

1. 将此插件文件夹复制到AstrBot的`plugins`目录下
2. 重启AstrBot服务

## 使用方法

### 基本命令

- `blackjack` - 查看21点游戏帮助
- `blackjack.create` - 创建新的PVE游戏
- `blackjack.create -n` - 创建新的PVP游戏（无庄家模式）
- `blackjack.end` - 强制结束当前游戏
- `blackjack.stats` - 查询个人战绩
- `blackjack.rank` - 查看盈亏排行榜

### 游戏流程

1. **创建游戏**: 使用 `blackjack.create` 创建PVE游戏或 `blackjack.create -n` 创建PVP游戏
2. **加入游戏**: 发送 `下注 <金额>` 加入游戏
3. **开始游戏**: 发送 `开始` 开始发牌
4. **游戏操作**:
   - `要牌` (`hit`/`h`) - 要一张牌
   - `停牌` (`stand`/`s`) - 停止要牌
   - `加倍` (`double`/`d`) - 双倍下注并要最后一张牌
   - `分牌` (`split`/`p`) - 如果手牌相同则分开
   - `投降` (`surrender`) - 投降并退回一半赌注
   - `保险` (`insurance`) - 在庄家明牌为A时购买保险

## 游戏规则

- **BJ赔率**: 21点（BJ）赔付3:2
- **庄家规则**: 庄家小于17点必须拿牌
- **分牌A规则**: 分裂A牌后每手只发一张牌

## 技术特点

- 使用Python 3.8+开发
- 基于AstrBot框架
- 支持多平台接入
- 异步非阻塞架构

## 作者

祁筱欣

## 许可证

GNU AFFERO GENERAL PUBLIC LICENSE Version 3 (AGPL-3.0)

## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fxiaomizhoubaobei%2Fastrbot_plugin_blackjack.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fxiaomizhoubaobei%2Fastrbot_plugin_blackjack?ref=badge_large)