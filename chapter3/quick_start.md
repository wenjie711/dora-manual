# 快速上手指南
## 创建一个Ufop
打开Dora数据处理平台web管理界面，点击左边导航条中的应用开发

![1](http://7xnvrp.com1.z0.glb.clouddn.com/ufop_quick_start_1.png)

点击右边大区域右上角的`创建新的应用`按钮
- 填写应用名称：`hello_world`
- 选择运行环境的配置：`M0C1`
- 填写描述：`My Hello World Ufop`
- 点击`确定`按钮

![2](http://7xnvrp.com1.z0.glb.clouddn.com/ufop_quick_start_2.png)

## 提交构建版本
点击刚刚创建的Ufop，选择右边大区域右上方的`版本`标签`

![3](http://7xnvrp.com1.z0.glb.clouddn.com/ufop_quick_start_3.png)

点击`新建版本`按钮
- 填写版本的描述：`My Hello World Ufop Version !!`
- 选择一个Ufop的tar包，tar包的格式要求请参考：...

![4](http://7xnvrp.com1.z0.glb.clouddn.com/ufop_quick_start_4.png)

版本构建需要一段时间，等版本成功构建后，将该号版本设成开发版本。

![5](http://7xnvrp.com1.z0.glb.clouddn.com/ufop_quick_start_5.png)

## 创建运行实例
当具有一个成功构建的版本，并且设置其为开发版本后，下面就可以创建运行的实例
您可以根据你的需求选择合适数量的实例数

![6](http://7xnvrp.com1.z0.glb.clouddn.com/ufop_quick_start_6.png)

调整实例个数需要一些时间，请耐心等待

![7](http://7xnvrp.com1.z0.glb.clouddn.com/ufop_quick_start_7.png)


## 访问和使用您的Ufop

至此，您已经完成了 Ufop 的创建和部署，现在您可以按以下的方式从外部访问您的 Ufop，这里以 `hello_world` 为例：

直接访问方式：

    http://demo.qiniudn.com/demo.txt?hello_world/<text-to-grep>

使用管道的方式访问（这里以 exif 的输出作为 hello_world 的输入）：

    http://demo.qiniudn.com/demo.jpg?exif|hello_world/<text-to-grep>

下面是在浏览器中访问Ufop的效果，该Ufop的效果是在Response中输出Hello

![8](http://7xnvrp.com1.z0.glb.clouddn.com/ufop_quick_start_8.png)

当然，如果使用管道，您可以在七牛的 fop 和您有权访问的所有 ufop 之间自由地组合搭配，得到您想要的处理结果。

