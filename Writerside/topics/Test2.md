# 人生书籍

1.寻找生命的意义 -高效人士的七个习惯的扩展材料

> **Highlight important information**
>
> You can change the element to *tip* or *warning* by renaming the style attribute below.
>
{style="note"}

## Before you start

It is good practice to list the prerequisites that are required or recommended.

Make sure that:
- First prerequisite
- Second prerequisite

## How to perform a task

Some introductory information.

1. Step with a code block

   ```bash
    run this --that
   ```

2. Step with a [link](https://www.jetbrains.com)

3. Step with a list.
   - List item
   - List item
   - List item
     //sphinx MYSQL的高性能全文检索系统

     //Archive引擎是一个例外，Archive引擎是一个例外：5.1之前Archive不支持任何索引，直到5.1才开始支持单个自增列(AUTO_INCREMENT)的索引。


        //索引是如何工作的？
        //索引类似一本书的目录部分

        //索引在MYSQL中哪一层实现的？ 有什么弊端？
        //在存储引擎层实现的，而不是服务器层实现的。没有统一索引的标准，因为不同引擎工作方式不一样，不是所有存储引擎都支持所有类型的索引。

        // B-Tree是什么？ 有什么特性？
        // 通常意味着所有的值都是按顺序存储的，并且每一个叶子页到根的距离相同

        // 有什么弊端？
        // 1.联合索引如果不按照从最左列开始查找，则无法使用索引。2.不能跳过索引中的列。3.如果对其中某一列的值做范围查询，则其右边的列无法使用索引。
        // 所以索引的列顺序很重要，优化性能时，我们需要使用相同的多个列，但是顺序不同来满足查询要求。