<!--
 * @Author: OBKoro1
 * @Github: https://github.com/OBKoro1
 * @Date: 2018-10-31 14:18:17
 * @LastEditors: OBKoro1
 * @LastEditTime: 2018-12-26 15:26:42
 -->

# 更新日志

## language

简体中文 | [English](https://github.com/OBKoro1/koro1FileHeader/wiki/change-log)

### [V3.3.0]

  * 新增配置[autoAlready](https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE#autoalready%E5%8F%AA%E8%AE%A9%E6%94%AF%E6%8C%81%E7%9A%84%E8%AF%AD%E8%A8%80%E8%87%AA%E5%8A%A8%E6%B7%BB%E5%8A%A0%E5%A4%B4%E9%83%A8%E6%B3%A8%E9%87%8A)：开启了[自动添加头部注释功能](https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE#2-%E8%87%AA%E5%8A%A8%E6%B7%BB%E5%8A%A0%E6%96%87%E4%BB%B6%E5%A4%B4%E9%83%A8%E6%B3%A8%E9%87%8A%E5%8F%AF%E9%80%89%E9%A1%B9)后,默认只给[支持语言](https://github.com/OBKoro1/koro1FileHeader/wiki/%E6%94%AF%E6%8C%81%E8%AF%AD%E8%A8%80)的文件自动添加头部注释。
    
    这是非常必要的，因为发现存在一些问题，了解[配置](https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE#autoalready%E5%8F%AA%E8%AE%A9%E6%94%AF%E6%8C%81%E7%9A%84%E8%AF%AD%E8%A8%80%E8%87%AA%E5%8A%A8%E6%B7%BB%E5%8A%A0%E5%A4%B4%E9%83%A8%E6%B3%A8%E9%87%8A)

### [V3.2.0]

  * 插件[支持根据文件后缀，头部注释插入到不同行](https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE#3-%E5%A4%B4%E9%83%A8%E6%B3%A8%E9%87%8A%E7%AC%AC%E5%87%A0%E8%A1%8C%E6%8F%92%E5%85%A5)，比如`php`:

        <?php
        // 第一行需要为`<?php`否则注释不生效
        /*
         * @Author: OBKoro1
         * @Github: https://github.com/OBKoro1
         * @Date: 2018-12-21 10:49:35
         * @LastEditors: OBKoro1
         * @LastEditTime: 2018-12-21 13:12:37
         * @Description: 
         */
        ?>

  * 插件新增支持`md`后缀文件的头部注释，效果如下:

        <!--
        * @Author: OBKoro1
        * @Github: https://github.com/OBKoro1
        * @Date: 2018-12-20 13:43:44
        * @LastEditors: OBKoro1
        * @LastEditTime: 2018-12-20 13:48:36
        * @Description: 
        -->
    我平常写`markdown`比较多，可以用于记录`md`的创建日期和修改日期。

  * 插件支持在线修改配置中的数据，修改配置，再也不用重启VsCode了！

  * 更新函数注释的默认配置,`msg`替换为`description`，这样`description`在VsCode中也会高亮：

        /**
         * @description: 
         * @param {type} 
         * @return: 
         */


### [V3.1.0]

  * 新增自动添加头部注释功能，再也不用担心忘记给文件添加头部注释了！前往[配置](https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE#2-%E8%87%AA%E5%8A%A8%E6%B7%BB%E5%8A%A0%E6%96%87%E4%BB%B6%E5%A4%B4%E9%83%A8%E6%B3%A8%E9%87%8A%E5%8F%AF%E9%80%89%E9%A1%B9)了解详情.

### [V3.0.0]

  * 新增自定义注释的符号，注释生成的样子，全部由你掌控，详情请看[插件配置](https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE#%E6%8F%92%E4%BB%B6%E9%85%8D%E7%BD%AE)。

  * 头部注释和函数注释现在**支持中文做为注释属性了**,比如：

        "fileheader.cursorMode": {
          "Date": "Do not edit",
          "作者": "your name",
          "功能": ""
        }

  * 函数注释新增Date字段，设置该字段可生成函数注释的时间

  * 修复文件行数不够20行时，无法更新最后编辑时间的bug

  * 修复函数注释在最后一行无法生成的bug

### [V2.9.0]

  * 插件新增支持`vue`后缀文件的头部注释，效果如下:

        <!--
        * @Description: 
        * @Author: OBKoro1
        * @Github: https://github.com/OBKoro1
        * @Date: 2018-11-16 14:38:05
        * @LastEditors: OBKoro1
        * @LastEditTime: 2018-11-19 14:32:45
        -->

### [V2.8.0]

  * 插件新增支持`html`后缀文件的头部注释，效果如下:

        <!--
        * @Description: 
        * @Author: OBKoro1
        * @Github: https://github.com/OBKoro1
        * @Date: 2018-11-16 14:38:05
        * @LastEditors: OBKoro1
        * @LastEditTime: 2018-11-19 14:32:45
        -->

### [V2.7.0]
  
  * 新增[WiKi](https://github.com/OBKoro1/koro1FileHeader/wiki),关于插件的文档都在这里!

  * 插件新增支持`vb`后缀文件注释,按下快捷键检测为`vb`后缀的文件,效果如下
    
        // 头部注释  
        '
        ' @Description: 
        ' @Author: OBKoro1
        ' @Github: https://github.com/OBKoro1
        ' @Date: 2018-11-08 11:09:02
        ' @LastEditTime: 2018-11-08 13:49:26
        '
        // 函数注释
        '
        ' description: 
        ' param {type} 
        ' return: 
        '
  * 修复必须`LastEditors`和`LastEditTime`字段同时存在才会更新最后编辑时间的bug
    
    同时存在或者单独使用`LastEditors`、`LastEditTime`字段都支持更新最后编辑时间和最后编辑人

  * 新增[支持注释格式](https://github.com/OBKoro1/koro1FileHeader/blob/master/document/supportNotes.md)

### [V2.6.0]

  * 新增[常见问题readme](https://github.com/OBKoro1/koro1FileHeader/blob/master/document/commonProblems.md)
  * 修复部分场景下最后编辑时间不更新问题
  * 对单个文件连续操作，最后编辑时间与上次的最后编辑时间相差6666毫秒才会更新

### [V2.5.0]

  * 支持python注释，按下快捷键检测为py后缀的文件，生成`'''`形式的文件头部注释和函数注释。
  * 头部注释Date字段(文件创建时间)从当前时间改为文件的创建时间

### [V2.0.0]

  * 新增在光标出添加注释功能(通常用于函数/方法注释)，同样的支持用户自定义注释选项
  * 修复文件头部注释的默认配置不可删除，配置顺序不可移动的问题
  * 新增mac快捷键