# Bu-PortScan

<img width="632" height="214" alt="image" src="https://github.com/user-attachments/assets/45af25af-a480-4a2b-ae72-d9f7cf6adbfa" />

Bu-PortScan 是一个简单高效的端口扫描工具，基于 Python 开发，支持多线程扫描和多种端口范围选择。

## 功能特点

- ✅ 支持多线程端口扫描
- ✅ 内置三种端口范围：Top100、Top1000、全端口
- ✅ 实时显示扫描结果
- ✅ 自动保存扫描结果到 CSV 文件
- ✅ 简洁的命令行交互界面
- ✅ 提供 Windows 可执行文件（exe）和 zip 打包版本

## 环境要求

### 直接运行 Python 脚本
- Python 3.6+
- 依赖库：
  - requests
  - rich

### 使用 zip 打包版本
- Windows 系统
- 无需安装 Python 环境

## 安装依赖

如果直接运行 Python 脚本，需要安装依赖：

```bash
pip install -r requirements.txt
```

## 使用方法

### 方法一：直接运行 Python 脚本

1. 运行程序：
   ```bash
   python Bu-PortScan.py
   ```

2. 选择功能：
   - 1. 输入目标进行端口扫描
   - 2. 设置线程数
   - 3. 设置端口字典
   - 4. 退出

### 方法二：使用 zip 打包版本

1. 解压 `Bu-PortScan_v1.0.0_win.zip` 文件
2. 双击运行解压目录中的 `Bu-PortScan.exe` 文件
3. 按照命令行提示进行操作

## 端口字典说明

- **Top100**：常用的 100 个端口
- **Top1000**：常用的 1000 个端口
- **全端口**：1-65535 所有端口

## 示例

```
请输入1.输入目标进行端口扫描 2.设置线程(当前:10) 3.设置字典(当前:top100) 4.退出: 1
请输入目标IP地址或url：
127.0.0.1
[*]端口[21]关闭
[*]端口[22]关闭
[*]端口[80]开放
[*]扫描完成!结果已保存到results\127.0.0.1.csv
[*]目标127.0.0.1开放端口:{80}
```

## 项目结构

```
Bu-PortScan/
├── Bu-PortScan.py         # 主程序（Python 源码）
├── Bu-PortScan_v1.0.0_win.zip  # Windows 打包版本（含 exe）
├── .gitignore        # Git 忽略文件
├── README.md         # 项目说明
├── logo.ico          # 程序图标
└── requirements.txt  # 依赖库
```

## 依赖库

创建 `requirements.txt` 文件：

```
requests
rich
```

## 注意事项

- 扫描全端口可能需要较长时间，请耐心等待
- 建议根据网络环境调整线程数，避免因线程过多导致网络阻塞
- 请遵守相关法律法规，不要对未经授权的目标进行扫描

## 许可证

本项目采用 MIT 许可证。

## 作者

Bu7terf1y

## 项目地址

[https://github.com/Bu7terf1y/Bu-PortScan](https://github.com/Bu7terf1y/Bu-PortScan)
