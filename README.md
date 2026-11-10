# Workspace Replay Kit

实验交付资料与中文执行说明。

## 获取完整交付包

打开 [v1.0.0 下载页](https://github.com/ytqing/replay-workspace-kit/releases/tag/v1.0.0)，下载全部七个`replay-workspace-kit-partNN-of07.zip`和五个配套文件到同一目录：

- restore_handoff.py
- upload_manifest.json
- SHA256SUMS.txt
- README.md
- verification_report.json

运行恢复工具：

```bash
python3 restore_handoff.py
```

Windows可运行`py -3.10 restore_handoff.py`。所有分包先验证，再恢复为`handoff/`目录。恢复后让接手agent读取其中的README.md和AGENTS.md，按一次任务授权完成环境准备、构建、验证、测量、分析与回传。

## 默认测量

本地batch size为128、512、2048、8192；36场景，四策略，五次独立进程重复，184320次计时调用。交付包包含固定源码、构建依赖、完整路由数据、强化正确性验证和报告工具。

完整附件约6.22GB，建议预留25GB工作空间。仓库本体仅提供下载入口，完整文件在Release附件中。
