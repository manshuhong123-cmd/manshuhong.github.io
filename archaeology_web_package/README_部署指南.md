# 考古勘探影像采集系统（网址版 / PWA）

## 文件说明
- `index.html`：主页面
- `manifest.webmanifest`：PWA 清单文件
- `sw.js`：离线缓存 Service Worker
- `icons/`：桌面图标
- `.nojekyll`：GitHub Pages 兼容文件

## 方式一：GitHub Pages（最简单）
1. 新建一个 GitHub 仓库
2. 把本目录全部文件上传到仓库根目录
3. 打开仓库 `Settings -> Pages`
4. `Build and deployment` 里选择：
   - Source: `Deploy from a branch`
   - Branch: `main`（或你实际使用的分支）
   - Folder: `/ (root)`
5. 保存后等待几分钟
6. 访问：`https://你的用户名.github.io/仓库名/`

> 如果你要让资源路径最稳，建议把仓库名改成：`archaeology-app`，然后访问类似：
> `https://yourname.github.io/archaeology-app/`

## 方式二：Cloudflare Pages
1. 登录 Cloudflare
2. 进入 Workers & Pages -> Create application -> Pages -> Upload assets
3. 直接上传本目录全部文件
4. 部署完成后会得到一个 `*.pages.dev` 网址

## 自定义域名
- GitHub Pages 和 Cloudflare Pages 都支持绑定你自己的域名
- 绑定后可开启 HTTPS，并更适合移动端相机与 PWA 使用

## 使用建议
- 手机访问 HTTPS 网址后，添加到主屏幕
- 现场拍照后及时导出 ZIP
- 如果单位长期使用，建议绑定独立域名，便于统一管理
