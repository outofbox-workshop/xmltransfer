# 剧本 CSV 转 XML 工具使用说明书 (v1.5)

## 1. 工具简介
本工具用于将策划编写的剧情 CSV 表格（`newdialog.csv`）批量转换为工程可用的 XML 格式（`output_new.xml`）。

**适用版本：** 适配 XML 转换规则 1.5
**主要功能：**
* **ID 自动映射**：自动处理 Character ID、Spine ID、Action ID、Background ID。
* **HCG 模式识别**：自动识别 HCG 场景（强制居中）与普通立绘模式（左/中/右）。
* **参数透传**：支持 `isLoop`、`spineScale`、`spineOffset` 等参数的直接读取。

---

## 2. 环境准备

在使用脚本前，请确保电脑上已安装 Python 环境。

### 第一步：安装 Python
如果未安装，请前往 [Python 官网](https://www.python.org/) 下载并安装。
> **⚠️ 重要提示：** 安装时务必勾选底部的 **"Add Python to PATH"** 选项。

### 第二步：安装依赖库
打开命令行工具（CMD 或 PowerShell），输入以下指令安装 `pandas` 库：
```bash
pip install pandas
