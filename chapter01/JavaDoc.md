title: 4-JavaDoc
date: 2021-08-22

# Java文档注释

## 概念

Java 支持三种注释方式。前两种分别是 // 和 /* */，第三种被称作文档注释，它以 /** 开始，以 */结束。

说明注释允许你在程序中嵌入关于程序的信息。你可以使用 JavaDoc 工具软件来生成信息，并输出到HTML文件中。

文档注释，使你更加方便的记录你的程序信息。

## cmd命令

``` bash
javadoc -d <s路径> -<需要生成的doc标签> <*.java>
```

![](https://hexo-4grmu8ecde66adf2-1306730064.tcloudbaseapp.com/pic/javadoc1.png)

随后会在上述文件夹里生成很多文件，点击index.html

![](https://hexo-4grmu8ecde66adf2-1306730064.tcloudbaseapp.com/pic/javadoc2.png)

详细内容如下

![](https://hexo-4grmu8ecde66adf2-1306730064.tcloudbaseapp.com/pic/javadoc3.png)

## JavaDoc标签

| 标签                    | 描述                                                   | 示例                                                         |
| ----------------------- | ------------------------------------------------------ | ------------------------------------------------------------ |
| @author                 | 标识一个类的作者                                       | @author Tom                                                  |
| @deprecated             | 指名一个过期的类或成员                                 | @deprecated tom                                              |
| @version                | 指定类的版本                                           | @version info                                                |
| @exception              | 标志一个类抛出的异常                                   | @exception exception-name explanation                        |
| @param                  | 说明一个方法的参数                                     | @param parameter-name explanation                            |
| @return                 | 说明返回值类型                                         | @return explanation                                          |
| @see                    | 指定一个到另一个主题的链接                             | @see anchor                                                  |
| @serial                 | 说明一个序列化属性                                     | @serial description                                          |
| @serialData             | 说明通过writeObject( ) 和 writeExternal( )方法写的数据 | @serialData description                                      |
| @serialData description | 说明一个ObjectStreamField组件                          | @serialField name type description                           |
| @since                  | 标记当引入一个特定的变化时                             | @since release                                               |
| @throws                 | 和 @exception标签一样                                  | The @throws tag has the same meaning as the @exception tag   |
| {@docRoot}              | 指明当前文档根目录的路径                               | Directory Path                                               |
| {@inheritDoc}           | 从直接父类继承的注释                                   | Inherits a comment from the immediate surperclass            |
| {@link}                 | 插入一个到另一个主题的链接                             | {@link name text}                                            |
| {@linkplain}            | 插入一个到另一个主题的链接，但是该链接显示纯文本字体   | 插入一个到另一个主题的链接，但是该链接显示纯文本字体         |
| {@value}                | 显示常量的值，该常量必须是static属性                   | Displays the value of a constant, which must be a static field |

