# 个人博客

[Runtime](https://github.com/Areaper/MyBlog/issues/1)

[UIDynamics](https://github.com/Areaper/MyBlog/issues/2)

[CoreImage](https://github.com/Areaper/MyBlog/issues/3)

[ReactiveCocoa](https://github.com/Areaper/MyBlog/issues/4)

[CoreData](https://github.com/Areaper/MyBlog/issues/5)

[计算机组成原理概论和总线](https://github.com/Areaper/MyBlog/issues/6)

[Swift中处理JSON](https://github.com/Areaper/MyBlog/issues/9)

[计算机存储器](https://github.com/Areaper/MyBlog/issues/8)

NSZombieEnabled变量用来调试与内存有关的问题，跟踪对象的释放过程。启用了NSZombieEnabled的话，它会用一个僵尸来替换默认的dealloc实现，也就是在引用计数降到0时，该僵尸实现会将该对象转换成僵尸对象。僵尸对象的作用是在你向它发送消息时，它会显示一段日志并自动跳入调试器。
所以，当在应用中启用NSZombie而不是让应用直接崩溃掉时，一个错误的内存访问就会变成一条无法识别的消息发送给僵尸对象。僵尸对象会显示接受到得信息，然后跳入调试器，这样你就可以查看到底是哪里出了问题。
可以在Xcode的scheme页面中设置NSZombieEnabled环境变量。点击Product——>Edit Scheme打开该页面，然后勾选Enable Zombie Objects 复选框。 
