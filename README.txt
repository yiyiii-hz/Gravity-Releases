Gravity 1.2.3 发布文件

- Gravity-1.2.3-macOS-arm64.zip
- Gravity-1.2.3-Windows-x64-Setup.exe
- Gravity-1.2.3-Windows-x64-Portable.zip
- latest.json
- SHA256SUMS（以上文件的 SHA-256）

校验：shasum -a 256 -c SHA256SUMS（Windows：certutil -hashfile <文件> SHA256）。
latest.json 是带 Ed25519 签名的更新清单，客户端内置公钥验证；不要手改。

发布步骤（手动，本脚本不会上传）：
1. 在 Gravity-Releases 创建 tag v1.2.3 的 Release，上传上面的安装包；
2. 把 latest.json 放到更新地址（GitHub Pages）；
3. 先用一台机器从旧版本走一遍应用内更新再通知客户。

产品口径：第一跳和第二跳都由客户自行购买，Gravity 只生成配置模板；不承诺防封、不承诺通过风控。

—— 本版本说明 ——
# Gravity 1.2.3

- 环境页新增「Claude 账号 KYC 状态」查询（独立登录窗口，非公开接口，仅供参考）。
- 第一跳和第二跳都由客户自行购买，Gravity 只生成配置模板；不承诺防封、不承诺通过风控。
