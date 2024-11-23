# BJTU-Homework-Tracker

![GitHub contributors](https://img.shields.io/github/contributors/ymzhang-cs/BJTU-Homework-Tracker)
![GitHub commit activity](https://img.shields.io/github/commit-activity/t/ymzhang-cs/BJTU-Homework-Tracker)
![GitHub last commit](https://img.shields.io/github/last-commit/ymzhang-cs/BJTU-Homework-Tracker)
![GitHub](https://img.shields.io/github/license/ymzhang-cs/BJTU-Homework-Tracker)

北京交通大学智慧课程平台作业抓取

支持在登录后自动化抓取作业列表，在筛选后进行可视化输出。

支持的登录方式：

- 智慧课程平台账号登录
- MIS 系统登录
- Cookie登录

支持的作业筛选方式

- 按完成状态：未完成/已完成/全部
- 按课程名：支持白名单/黑名单
- 按距离截止时间
- 按已过期时间

支持的显示/保存结果方式

- HTML页面渲染
- 纯文本显示

## 快速上手

0. 克隆仓库

```bash
git clone https://github.com/ymzhang-cs/BJTU-Homework-Tracker.git
cd BJTU-Homework-Tracker
```

1. 安装依赖

```bash
pip install -r requirements.txt
```

2. 配置config.yaml（可选，推荐）

参考config_sample.yaml的注释填写即可。

3. 运行

```bash
python run.py
```

> [!NOTE]
> 如果选择使用 MIS 系统登录，请确保已经安装了 Chrome 浏览器或 Edge 浏览器（后续会支持更多）。
> 
> 第一次使用会自动下载对应的 WebDriver，如果下载失败请手动下载并放置在浏览器根目录（如 `C:\Program Files\Google\Chrome\Application`）下。

## TODO

- [ ] 使用 Schema 验证配置文件 [#8](https://github.com/ymzhang-cs/BJTU-Homework-Tracker/issues/8)
- [ ] 更好的 WebDriver 配置模式 [#9](https://github.com/ymzhang-cs/BJTU-Homework-Tracker/issues/9)
- [ ] 考虑使用 PyInquirer 交互式配置 [#16](https://github.com/ymzhang-cs/BJTU-Homework-Tracker/issues/16)

## 参考资料

[如何获取Cookie](FOR_NEWERS.md)