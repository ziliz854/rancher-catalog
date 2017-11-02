# TensorFlow (CPU only)

### 说明

本应用将安装Tensorflow的执行环境，并配置"jupyter", "tensorboard"来进行交互操作。

部署本应用需要配置NoteBook登陆密码和Log目录，对于用户自己的notebook，需要在代码中设置log的输出路径为该指定的路径，以实现TensorBoard的可视化。

部署完成后可以通过`8888`端口访问NoteBook，通过`6006`端口访问TensorBoard。

### 预定义环境变量

本应用部署后设置了如下环境变量，供用户在写python代码时使用，具体的变量值可在用户申请该应用时配置

| 环境变量 | 默认值 | 说明 |
| ------- | ------- | ------- |
| LOG_DIR | `/tmp/tensorflow_logs` | log路径，将TensorFlow运行的汇总数据输出到这个路径后，可以打开TensorBoard查看可视化数据 |
| DATA_DIR | `/tmp/tensorflow_data` | data路径，用于存放训练用和测试用数据的临时目录 |