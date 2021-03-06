# 贡献指南

> 请您勇敢地去翻译和改进翻译。虽然我们追求卓越，但我们并不要求您做到十全十美，因此请不要担心因为翻译上犯错——在大部分情况下，我们的服务器已经记录所有的翻译，因此您不必担心会因为您的失误遭到无法挽回的破坏。（改编自维基百科）

负责人：

+   [飞龙](https://github.com/wizardforcel)：562826179

## 章节列表

+   [1. 用户手册](docs/11.md)
    +   [1.1。 Numba 的约 5 分钟指南](docs/12.md)
    +   [1.2。概述](docs/13.md)
    +   [1.3。安装](docs/14.md)
    +   [1.4。使用`@jit` 编译 Python 代码](docs/15.md)
    +   [1.5。使用`@generated_jit` 进行灵活的专业化](docs/16.md)
    +   [1.6。创建 Numpy 通用函数](docs/17.md)
    +   [1.7。用@jitclass 编译 python 类](docs/18.md)
    +   [1.8。使用`@cfunc` 创建 C 回调](docs/19.md)
    +   [1.9。提前编译代码](docs/20.md)
    +   [1.10。使用`@jit` 自动并行化](docs/21.md)
    +   [1.11。使用`@stencil`装饰器](docs/22.md)
    +   [1.12。从 JIT 代码  中回调到 Python 解释器](docs/23.md)
    +   [1.13。性能提示](docs/24.md)
    +   [1.14。线程层](docs/25.md)
    +   [1.15。故障排除和提示](docs/26.md)
    +   [1.16。常见问题](docs/27.md)
    +   [1.17。示例](docs/28.md)
    +   [1.18。会谈和教程](docs/29.md)
+   [2. 参考手册](docs/30.md)
    +   [2.1。类型和签名](docs/31.md)
    +   [2.2。即时编译](docs/32.md)
    +   [2.3。提前编译](docs/33.md)
    +   [2.4。公用事业](docs/34.md)
    +   [2.5。环境变量](docs/35.md)
    +   [2.6。支持的 Python 功能](docs/36.md)
    +   [2.7。支持的 NumPy 功能](docs/37.md)
    +   [2.8。与 Python 语义的偏差](docs/38.md)
    +   [2.9。浮点陷阱](docs/39.md)
    +   [2.10。 Python 2.7 寿命终止计划](docs/40.md)
+   [3. 用于 CUDA GPU 的 Numba](docs/41.md)
    +   [3.1。概述](docs/42.md)
    +   [3.2。编写 CUDA 内核](docs/43.md)
    +   [3.3。内存管理](docs/44.md)
    +   [3.4。编写设备功能](docs/45.md)
    +   [3.5。 CUDA Python 中支持的 Python 功能](docs/46.md)
    +   [3.6。支持的原子操作](docs/47.md)
    +   [3.7。随机数生成](docs/48.md)
    +   [3.8。设备管理](docs/49.md)
    +   [3.10。示例](docs/50.md)
    +   [3.11。使用 CUDA 模拟器  调试 CUDA Python](docs/51.md)
    +   [3.12。 GPU 减少](docs/52.md)
    +   [3.13。 CUDA Ufuncs 和广义 Ufuncs](docs/53.md)
    +   [3.14。共享 CUDA 内存](docs/54.md)
    +   [3.15。 CUDA 阵列接口](docs/55.md)
    +   [3.16。 CUDA 常见问题](docs/56.md)
+   [4. CUDA Python 参考](docs/57.md)
    +   [4.1。 CUDA 主机 API](docs/58.md)
    +   [4.2。 CUDA 内核 API](docs/59.md)
    +   [4.3。内存管理](docs/60.md)
+   [5. 用于 AMD ROC GPU 的 Numba](docs/61.md)
    +   [5.1。概述](docs/62.md)
    +   [5.2。编写 HSA 内核](docs/63.md)
    +   [5.3。内存管理](docs/64.md)
    +   [5.4。编写设备功能](docs/65.md)
    +   [5.5。支持的原子操作](docs/66.md)
    +   [5.6。代理商](docs/67.md)
    +   [5.7。 ROC Ufuncs 和广义 Ufuncs](docs/68.md)
    +   [5.8。示例](docs/69.md)
+   [6. 扩展 Numba](docs/70.md)
    +   [6.1。高级扩展 API](docs/71.md)
    +   [6.2。低级扩展 API](docs/72.md)
    +   [6.3。示例：间隔类型](docs/73.md)
+   [7. 开发者手册](docs/74.md)
    +   [7.1。贡献给 Numba](docs/75.md)
    +   [7.2。 Numba 建筑](docs/76.md)
    +   [7.3。多态调度](docs/77.md)
    +   [7.4。关于发电机的注意事项](docs/78.md)
    +   [7.5。关于 Numba Runtime 的注意事项](docs/79.md)
    +   [7.6。使用 Numba Rewrite Pass 获得乐趣和优化](docs/80.md)
    +   [7.7。实时变量分析](docs/81.md)
    +   [7.8。上市](docs/82.md)
    +   [7.9。模板注释](docs/83.md)
    +   [7.10。关于自定义管道的注意事项](docs/84.md)
    +   [7.11。环境对象](docs/85.md)
    +   [7.12。哈希  的注意事项](docs/86.md)
    +   [7.13。 Numba 项目路线图](docs/87.md)
+   [8. Numba 增强建议](docs/88.md)
+   [9. 术语表](docs/89.md)

## 流程

### 一、认领

首先查看[整体进度](https://github.com/apachecn/numba-doc-zh/issues/1)，确认没有人认领了你想认领的章节。
 
然后回复 ISSUE，注明“章节 + QQ 号”（一定要留 QQ）。

### 二、翻译

可以合理利用翻译引擎（例如[谷歌](https://translate.google.cn/)），但一定要把它变得可读！

如果遇到格式问题，请随手把它改正。

### 三、提交

+   `fork` Github 项目
+   将译文放在`docs`文件夹下
+   `push`
+   `pull request`

请见 [Github 入门指南](https://github.com/apachecn/kaggle/blob/master/docs/GitHub)。
