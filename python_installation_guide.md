# Python 环境配置指南

## 一、下载 Python

1. 访问 Python 官方网站：https://www.python.org/downloads/
2. 选择适合您操作系统的版本（建议下载 Python 3.10 或更高版本）
3. 点击 "Download" 按钮开始下载

## 二、安装 Python

### Windows 系统

1. 双击下载的安装包
2. 在安装界面勾选 "Add Python to PATH" 选项（非常重要）
3. 点击 "Install Now" 进行默认安装
   - 也可以选择「Customize installation」进行自定义安装
4. 等待安装完成
5. 点击 "Close" 关闭安装窗口

### macOS 系统

1. 双击下载的 .pkg 文件
2. 按照安装向导的提示进行操作
3. 等待安装完成

### Linux 系统

大多数 Linux 发行版已经预装了 Python，您可以通过以下命令检查版本：

```bash
python3 --version
```

如果需要安装或升级，可以使用包管理器：

- Ubuntu/Debian:
  ```bash
  sudo apt update
  sudo apt install python3 python3-pip
  ```

- CentOS/RHEL:
  ```bash
  sudo yum install python3 python3-pip
  ```

## 三、验证 Python 安装

1. 打开命令提示符（Windows）或终端（macOS/Linux）
2. 输入以下命令检查 Python 版本：
   ```bash
   python --version
   ```
   或
   ```bash
   python3 --version
   ```
3. 输入以下命令检查 pip 版本：
   ```bash
   pip --version
   ```
   或
   ```bash
   pip3 --version
   ```

如果能正常显示版本号，则说明 Python 安装成功。

## 四、启动本地 HTTP 服务器

1. 打开命令提示符（Windows）或终端（macOS/Linux）
2. 使用 `cd` 命令进入您的项目目录：
   ```bash
   cd path/to/your/project
   ```
3. 输入以下命令启动本地 HTTP 服务器：
   ```bash
   python -m http.server 8080
   ```
   或
   ```bash
   python3 -m http.server 8080
   ```
4. 服务器启动后，在浏览器中输入以下地址访问您的项目：
   ```
   http://localhost:8080
   ```

## 五、常见问题及解决方案

### 问题 1：在 Windows 系统中，命令提示符显示 "python 不是内部或外部命令，也不是可运行的程序或批处理文件"

**解决方案**：
1. 检查是否在安装时勾选了 "Add Python to PATH" 选项
2. 如果没有勾选，重新运行安装包，选择 "Modify" 选项，然后勾选 "Add Python to PATH"
3. 或者手动将 Python 安装目录添加到系统环境变量中

### 问题 2：在 macOS/Linux 系统中，运行 `python` 命令时显示 Python 2.x 版本

**解决方案**：
- 使用 `python3` 命令代替 `python` 命令
- 使用 `pip3` 命令代替 `pip` 命令

### 问题 3：本地 HTTP 服务器启动失败

**解决方案**：
1. 检查端口是否被占用，可以尝试使用其他端口，如：
   ```bash
   python -m http.server 8081
   ```
2. 检查是否有足够的权限启动服务器

## 六、其他资源

- Python 官方文档：https://docs.python.org/zh-cn/3/
- Python 入门教程：https://www.runoob.com/python3/python3-tutorial.html
- pip 官方文档：https://pip.pypa.io/en/stable/

祝您使用 Python 愉快！