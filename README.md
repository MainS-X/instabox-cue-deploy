# MANUS CUE 云端 Android 自动化部署套件

本仓库提供在云端 Linux / Android 沙箱（如 [InstaBox](https://instabox.sh)、Redroid 容器环境）中全自动部署与运行 **MANUS CUE**（`ai.manus.agents`）的完整环境补丁包与初始化脚本。

通过预置的容器配置、机型伪装与 Dalvik 字节码补丁，彻底解决原生 CUE 在云端虚拟化安卓中的闪退、渲染崩溃与输入法卡顿问题。

---

## ⚡ 极速一键部署（约 60 秒）

在任何具备 Docker 与 ADB 的 Android 沙箱实例终端中，运行以下单行命令即可完成一键部署：

```bash
curl -sL https://github.com/<你的用户名>/<你的仓库名>/releases/download/v1.0.0/cue_deploy_bundle.tar.gz | tar -xz -C /tmp && bash /tmp/cue_package/install_cue.sh