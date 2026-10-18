# 手游行业情报日报站点

此仓库用于独立发布手游行业情报 HTML，预期访问域名：`https://new.lirare.xyz/`。

## 页面

- 首页：`index.html` → `https://new.lirare.xyz/`
- 首期：`2026-10-18/index.html` → `https://new.lirare.xyz/2026-10-18/`

## 首次开通（仓库拥有者在 GitHub / DNS 控制台完成）

1. 在仓库 `linirare/all` 的 **Settings → Pages** 中，把 Build and deployment 的 Source 设为 **Deploy from a branch**，Branch 选择 `main`、目录 `/ (root)`，点击 Save。
2. 在 **Custom domain** 检查或设置 `new.lirare.xyz`；仓库根目录已有 `CNAME` 文件，内容为 `new.lirare.xyz`。如果 GitHub 自动识别，确保页面显示一致即可。
3. 在 `lirare.xyz` 的 DNS 管理面板中新建记录：**类型 CNAME、主机记录 new、记录值 linirare.github.io**。若已有同名记录，请先核实后调整，避免重复冲突。Cloudflare 用户可以先用 DNS only 进行排查。
4. 待 DNS 与证书生效后，在 GitHub Pages 勾选 **Enforce HTTPS**。

请勿修改 `linirare/lirare-all-html` 原仓库的 `CNAME` (`gh.lirare.xyz`)，避免影响旧项目。

## 更新日报

每天新增一个 `YYYY-MM-DD/index.html`，同步在根目录的 `index.html` 中添加当期入口。
