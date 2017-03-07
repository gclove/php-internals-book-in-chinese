# 基础结构
 一个zval（“Zend value”的缩写）代表一个任意类型的PHP变量。所以，它很可能是PHP中最重要的数据结构，同时你将会频繁地使用它。本章节讲述zvals的基础概念及其使用方法。

## 类型和值
 每一个zval都会存储某个值和其对应的类型。这点非常重要，因为PHP是一门动态类型语言，所以变量的类型只有当运行时才会确定，并不是在编译时就能够确定。此外，zval的类型在其生命周期是可以改变的，所以如果这个zval在最初存储了一个整形，那么在之后的某个时间点他也可能会存储了一个字符串。