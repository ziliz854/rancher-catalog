## TensorFlow

TensorFlow 提供`Jupyter Notebook`, `TensorBoard`来进行交互操作。

### 访问方式:
 * <a href="{$T.publicEndpoints.jupyter_8888.url}" target="_blank">Jupyter Notebook</a>
 * <a href="{$T.publicEndpoints.jupyter_6006.url}" target="_blank">TensorBoard</a>

### 预定义环境变量

本应用部署后设置了如下环境变量，供用户在写python代码时使用，具体的变量值可在用户申请该应用时配置

| 环境变量 | 默认值 | 说明 |
| ------- | ------- | ------- |
| LOG_DIR | `/tmp/tensorflow_logs` | log路径，将TensorFlow运行的汇总数据输出到这个路径后，可以打开TensorBoard查看可视化数据 |
| DATA_DIR | `/tmp/tensorflow_data` | data路径，用于存放训练用和测试用数据的临时目录 |

#### python中获取环境变量方法：

```python
# 获取环境变量值：

log_dir = os.getenv('LOG_DIR', '/tmp/logs')
```
