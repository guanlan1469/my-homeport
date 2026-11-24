# my-homeport

个人 Shadowrocket 静态住宅 IP 分流模块（基于 [0xkaka/homeport](https://github.com/0xkaka/homeport) 扩展）。

## 模块订阅链接

```text
https://raw.githubusercontent.com/guanlan1469/my-homeport/main/homeport.module
```

## Shadowrocket 使用步骤

1. **导入并启用模块**：`配置 → 模块 → ＋` 粘贴上方链接下载，确认开关已开启。
2. **添加住宅节点**：类型选 `Socks5`（或 `HTTP`），填好代理地址、端口、完整用户名、密码，备注严格填写 **`🏠住宅出口-勿选`**。
3. **设置跳板**：点 `🏠住宅出口-勿选` 右侧 `ⓘ → 代理通过`，选一个稳定的原梯子节点。
4. **切换配置模式**：首页选中**原梯子节点**（不要选 `🏠住宅出口-勿选`），**全局路由**设为 **配置**，断开重连即可。

## 日常新增域名

直接编辑本仓库的 `homeport.module`，在 `[Rule]` 下新增一行并提交：

```ini
DOMAIN-SUFFIX,example.com,🏠住宅出口-勿选
```

提交后等 1～5 分钟（GitHub Raw 缓存），在各设备小火箭的 `配置 → 模块` 左滑点 **更新** 即可同步。
