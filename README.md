新的登录系统
=

    对原来的系统做了分层的优化

新的功能
-

并没有添加, 什么新的功能, 只是多了一个新的昵称选项

新的数据库
-

尝试了MySQL的数据库, 不知道为什么, 在第一次连接的时候, 总是异常的慢, 是不是以后的连接就不会在经过层层的步骤, 而是直连? 还没查阅过相关的资料<br/>
我在FormMain_load事件里面添加了连接的的东西, 但是在后续需要连接数据库的时候, 还是异常的慢, 等的我...<br/>
但是SQLserver就似乎好了一点??巨硬做的不错呵, MySQL是不是因为被甲骨文简介收购了之后, 在内部竞争中失败了??<br/>

内容的迁移
-

还没有将原来在SQLserver上面的数据迁移到MySQL里面, 到时候再说吧, 看看有没什么简单的方法, 不需要在自己去写程序<br/>
还写一个程序, 从SQLserver里面把省市区的的信息重新排了一下, 传到了MySQL的新表里面, 还是挺有意思的<br/>

接口的应用
-

因为要从子窗体向父窗体里面传递数据, 所以尝试了一丢丢的Interface的应用, 很有意思<br/>
这是肯定要学的东西 窗体之间的互相通信是一个程序的基本功能嘛, 肯定是要融汇贯通<br/>

删除了数据库连接的源码
-

似乎感觉将连接数据库的源码放在这边不是太安全啊, 就删去了源码, 添加了编译后的dll文件...<br/>

添加头像
-

添加的头像需要的事情, 比如说头像的BLOB的存储, 文件存储路径的存储,读取, 感觉就是在添加功能的路上一去不复返啊<br/>
还想添加头像剪切的功能, 感觉甚是复杂啊...<br/>

内心OS
-

为了避免数据库连接的密码泄露, 删除了原来的代码库, 搞得我好想好几天没有commit...<br/>
好尴尬, 原来的commit也没了, 难受, 我这么爱撸代码的人, 看着那 几天空空的很是难受啊...<br/>
