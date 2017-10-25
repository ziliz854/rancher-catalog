TensorFlow (CPU only)
===

### 说明

本应用将安装Tensorflow的执行环境，并配置"jupyter", "tensorboard"来进行交互操作。

部署本应用需要配置NoteBook登陆密码和Log目录，对于用户自己的notebook，需要在代码中设置log的输出路径为该指定的路径，以实现TensorBoard的可视化。

部署完成后可以通过`8888`端口访问NoteBook，通过`6006`端口访问TensorBoard。