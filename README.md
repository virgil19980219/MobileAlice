# MobileAlice - 手机股票页面复刻

这是一个复刻的手机股票页面项目，使用iPhone 15的屏幕尺寸，实现了股票行情展示、K线图绘制和买卖盘口等功能。

## 项目特点

- 使用iPhone 15屏幕尺寸（393px × 852px）
- 黑色主题设计
- Canvas绘制的实时K线图
- 买卖盘口展示
- 响应式布局设计

## 文件结构

- `stock_page.html` - 主页面文件，包含HTML、CSS和JavaScript代码
- `python_installation_guide.md` - Python环境配置指南
- `.gitignore` - Git忽略文件配置

## 如何使用

1. 安装Python环境（参考`python_installation_guide.md`）
2. 在项目目录下启动本地HTTP服务器：
   ```bash
   python -m http.server 8080
   ```
3. 在浏览器中访问：`http://localhost:8080/stock_page.html`

## 技术栈

- HTML5
- CSS3
- JavaScript (ES6+)
- Canvas API

## 功能模块

1. 顶部状态栏
2. 股票标题栏
3. 股票基本信息
4. 行情标签栏
5. K线图和买卖盘口（并排布局）
6. 底部导航栏
7. 投资者问答
8. 底部功能栏
9. Alice简报

## 许可证

MIT