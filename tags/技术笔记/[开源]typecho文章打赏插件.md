---
title: [开源]typecho文章打赏插件
date: 2021-03-12 13:31:48
tags:技术笔记
---

# [开源]typecho文章打赏插件

开源协议： Apache License 2.0
开源地址：[typecho-plugin](https://github.com/roomanl/typecho-plugin)

作者：[山顶洞洞人](http://rootvip.cn/archives/39.html#comment-45)

解压放到usr/plugins目录下，后台启用即可
然后在主题下面post.php文件里的文章末尾添加如下代码

```php
<?php Typecho_Plugin::factory('rootvip.cn.Donate')->Donate(); ?>
```

![请输入图片描述](https://sddman.oss-cn-shenzhen.aliyuncs.com/typecho/TIM%E6%88%AA%E5%9B%BE20200403181241.jpg)

插件配置如下：
![请输入图片描述](https://sddman.oss-cn-shenzhen.aliyuncs.com/typecho/TIM%E6%88%AA%E5%9B%BE20200403181339.jpg)

效果：

![image-20200605175306026](C:\Users\23333\AppData\Roaming\Typora\typora-user-images\image-20200605175306026.png)

如果typecho主题中开启了pjax，请在```<?php Typecho_Plugin::factory('rootvip.cn.Donate')->Donate(); ?>```下面加以下代码：

```<?php echo'<script>initDonate()</script>'?>```

![image-20200605174257483](C:\Users\23333\AppData\Roaming\Typora\typora-user-images\image-20200605174257483.png)

即可畅享丝滑，博主使用至今没有出现别的bug了，用着很舒服=-=