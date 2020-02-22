---
title: "面试官：为什么要重写hashcode和equals方法?"
date: 2020-02-22T12:09:24+08:00
draft: true
---
因为如果使用自定义对象作为hashmap的key，他的hashcode和equals不重写的话，hashcode则使用Object父类的方法返回的值为自定义对象的内存地址，equals方法也是一样，不重写，比较的就是内存地址的比较。所以应该重写这两个方法，给自定义对象添加类似用户id的int属性，再用这个属性去重写方法。
.


　　　转自微信公众号:CodeSheep