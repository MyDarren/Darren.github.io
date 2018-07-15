# 基本语法

## 换行
行尾加两个空格，然后加`return`键  
 
* 不换行  
`测试`  
`哈哈`

	效果如下：  
	```
	测试 哈哈
	```

* 换行    
`测试` ` ` ` `  
`哈哈`

	效果如下：  
	```
	测试
	哈哈
	```

## 加粗
加粗字前后都使用两个`*`号或者`_`    
`**加粗**`  
`__加粗__`

效果如下：  
>加粗  
**加粗**    
__加粗__

## 斜体
在斜体字前后加一个`*`号或者`_`    
`*斜体*`  

效果如下：  
>_斜体_

## 标题  
* 一种方式：一级标题可以在标题下一行使用`=`号，二级标题可以在标题下一行使用`-`号
* 另一种方式：总共可以有六级标题，分别在标题前面使用1-6个`#`号分别表示对应的标题等级  
`一级标题`  
`=`  
`二级标题`  
`-`

	效果如下：  
	>一级标题    
	>=  
	>二级标题  
	>-

	或者  
	`# 一级标题`  
	`## 二级标题`  
	`### 三级标题`  
	`#### 四级标题`  
	`##### 五级标题`  
	`###### 六级标题`  

	效果如下：  
	># 一级标题
	>## 二级标题
	>### 三级标题
	>#### 四级标题
	>##### 五级标题
	>###### 六级标题

## 链接和邮箱
* 自动链接，在链接前后使用`<>`  
  `<http://www.baidu.com>`  
  `<uranusjr@gmail.com>`

  效果如下：  
  ><http://www.baidu.com>  
  <uranusjr@gmail.com>      
* 行内链接`[]()`，`[]`里面为链接标题，`()`里面为链接地址  
  `[百度](http://www.baidu.com)`

  效果如下：    
  >[百度](http://www.baidu.com)
* 引用链接`[][]`，`[]:***`，其中第一个`[]`里面为链接标题，第二个`[]`里面为链接标识id，第三个`[]`里面链接标识id，其后面为真实url  
  `[GitHub](gitHub_id)`  
  `[gitHub_id]:https://github.com`

  效果如下：  
  >[GitHub](https://github.com)

## 图片
* 行内链接，使用`[]()`里面为图片本地或网络地址，地址后面可选图片标题
* 引用链接，使用`![][],[]:***`，其中第一个`[]`里面为图片标题，第二个`[]`里面为图片标识id，第三个`[]`里面为图片标识id，其后面为图片本地或网络地址，地址后面可选图片标题  
  `![网络图片1] (http://upload-images.jianshu.io/upload_images/1768589-173b2734f0487253.jpg "net_image1")` 
  
  效果如下：  
  >![网络图片1](http://upload-images.jianshu.io/upload_images/1768589-173b2734f0487253.jpg "net_image1")

  `![网络图片2][net_image]`  
  `[net_image]:https://imgt.388g.com/allimg/160711/5-160G10T615.jpg "net_image2"` 
  
  效果如下：  
  >![网络图片2][net_image]

  `![本地图片1] (local_image.jpg "local_image1")`  
  
  效果如下：  
  >![本地图片1](local_image.jpg "local_image1")

  `![本地图片2][local_image]`  
  `[local_image]:https://upload-images.jianshu.io/upload_images/1768589-d4c7faea86df4437.gif "local_image2"`  
  
  效果如下：      
  ![本地图片2][local_image]

## 列表
* 列表前必须有空行(或块元素)
* 无序列表使用`*`或`-`
* 列表内条目可以使用缩进进行嵌套
	- 无序列表
		- 一级嵌套
			- 二级嵌套
				- 三级嵌套

* 有序列表可以使用数字+`.`+空格的方式标识顺序
	- 有序列表
		1. 序号1
		2. 序号2
		3. 序号3

## 引用
* 使用`>`进行引用，只要段落之间没有空行，并不是每一行都需要以>开头  
  `> 筚路蓝缕，以启山林`  
  `君子和而不同，小人同而不和`  
  `德不孤，必有邻`
  
  `> 己所不欲，勿施于人`

  效果如下：  
  > 筚路蓝缕，以启山林  
  君子和而不同，小人同而不和  
  德不孤，必有邻
  
  > 己所不欲，勿施于人

* 引用可以嵌套  
  `> 三军可夺帅也，匹夫不可夺志也`  
  `> > 见贤思齐焉，见不贤而内自省也`  
  `> > > 朝闻道，夕死可矣`

  效果如下：  
  > 三军可夺帅也，匹夫不可夺志也  
  > > 见贤思齐焉，见不贤而内自省也  
  > > > 朝闻道，夕死可矣

* 大部分Markdown语法都可以在块引用中使用  
  `> * 列表`  
  `[百度](https://www.baidu.com)`  
  `![图片](http://upload-images.jianshu.io/upload_images/1768589-b07325f8a8178d14.jpg)`  
  `[简书][jianshu_id]`  
  `[jianshu_id]:https://www.jianshu.com`

  效果如下：  
  > * 列表  
  [百度](https://www.baidu.com)  
  ![图片](http://upload-images.jianshu.io/upload_images/1768589-b07325f8a8178d14.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)  
  [简书][jianshu_id]  

## 代码
* 行内代码，行内代码使用`` ` ``表示，如果代码中有反引号``code has `backticks ` ``需要显示，可以使用双反引号```` ``code has `backticks` `` ````
* 缩进代码，缩进代码可以使用至少4个空格或者1个Tab回退
  >` ` ` ` ` ` ` `print('缩进代码')  
  ` ` ` ` ` ` ` `print('缩进代码前必须有空白行')

  效果如下：  
  ```
      print('缩进代码')  
      print('缩进代码前必须有空白行')
  ```

* 代码块
    * 在代码前后使用`` ` ``
      >\`\`\`  
      print('代码块')  
      \`\`\`  

      效果如下：    
      ```  
      print('代码块')  
      ```  
    * 也可以使用`~`代替`` ` ``  
      >\~\~\~  
      print('代码块')  
      \~\~\~

      效果如下：  
      ```
      print('代码块')
      ```  
    * 在第一列末尾加上language ID支持代码高亮，支持的语言及语言id见[链接](http://macdown.uranusjr.com/features/code-block-highlighting/)
      >\~\~\~python  
      foo = (1,2,3,4)  
      bar = (5,6,7,8)  
      for f,b in zip(foo,bar):  
      ` ` ` ` ` ` ` `print f,b  
      \~\~\~

      效果如下：
          
      ``` python  
      foo = (1,2,3,4)     
      bar = (5,6,7,8)    
      for f,b in zip(foo,bar):    
          print f,b    
      ```  
      
      >\`\`\`objective-c  
      \- (void)testFunction{  
      ` ` ` ` ` ` ` `for (UIView *view in self.view.subviews) {  
      ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` `NSLog(@"%@",NSStringFromCGRect(view.frame));  
      ` ` ` ` ` ` ` `}  
      }   
      \`\`\`  
      
      效果如下：
        
      ```objective-c  
      - (void)testFunction{  
          for (UIView *view in self.view.subviews) {  
              NSLog(@"%@",NSStringFromCGRect(view.frame));  
          }  
      }  
      ```

## 水平线
使用在一行中使用`***`或者`---`，则会显示一条水平线
效果如下：
***
---

## 表格
* 使用`|`分割不同的列，在第一列下面使用`---`分割不同的行，使用:设置对其方式，表格前面必须有空白行
  ```
  First Column|Second Column
  ---|---
  年龄|18
  性别|男
  民族|汉
  ```
  效果如下：
  
  First Column|Second Column
  ---|---
  年龄|18
  性别|男
  民族|汉

* 最左边和最右边的管道`|`只是美观性的，可以省略；每一行排版并不重要，对齐完全取决于`:`标记，表格的列宽是由内容决定
  ```
  | Left Aligned  | Center Aligned  | Right Aligned |
  |:------------- |:---------------:| -------------:|
  | col 3 is      | some wordy text |         $1600 |
  | col 2 is      | centered        |           $12 |
  | zebra stripes | are neat        |            $1 |
  ```
  效果如下：
  
  | Left Aligned  | Center Aligned  | Right Aligned |
  |:------------- |:---------------:| -------------:|
  | col 3 is      | some wordy text |         $1600 |
  | col 2 is      | centered        |           $12 |
  | zebra stripes | are neat        |            $1 |

* 下面是支持的可选内联标记的列表
  ```
  Option name         | Markup            | Result if enabled     |
  --------------------|-------------------|-----------------------|
  Intra-word emphasis | So A\*maz\*ing    | So A<em>maz</em>ing   |
  Strikethrough       | \~~Much wow\~~    | <del>Much wow</del>   |
  Underline           | \_So doge\_       | <u>So doge</u>        |
  Quote [^quote]      | \"Such editor\"   | <q>Such editor</q>    |
  Highlight           | \==So good\==     | <mark>So good</mark>  |
  Superscript         | hoge\^(fuga)      | hoge<sup>fuga</sup>   |
  Autolink            | http://t.co       | <http://t.co>         |
  Footnotes           | [\^4]: and [\^4]: | [^4] and footnote 4  |
  ```
  
  Option name |   Markdown Markup   | Result if enabled
  ------------| --------------------| ----------------
  斜体         | So A\*maz\*ing      |So A<em>maz</em>ing
  删除线       |\~\~Much wow\~\~     |<del>Much wow</del>
  下划线       |\\\_So doge\\\_      |<u>So doge</u>  
  引用\[^quote\] |"Such editor"      |<q>Such editor</q>
  高亮         |==So good==          |<mark>So good</mark>
  上标         |hoge^fuga            |hoge<sup>fuga</sup> 
  链接         |http://t.co          |<http://t.co>  
  脚注         |\[\^foot]            |[^foot]  

  
  \[^foot]: You don't have to use a number. Arbitrary things like `[^footy note4]` and `[^footy note4]:` will also work. But they will *render* as numbered footnotes. Also, no need to keep your footnotes in order, I will sort out the order for you so they appear in the same order they were referenced in the text body. You can even keep some footnotes near where you referenced them, and collect others at the bottom of the file in the traditional place for footnotes. 

  \[^foot]: 脚注不需要一定用数字。任意的`[footy note4]`和`[footy note4]:`都有效，他们会按照脚注的id渲染，在文中使用了`[^foot]`标记脚注后，只有在后面用`[^foot]: `备注脚注后才能让该脚注渲染。同样的不需要保持脚注备注的顺序，Markdown将为你整理一下顺序，这样它们就会按照在文本正文中引用的顺序出现；甚至可以在引用它们的地方附近保留一些脚注，也可以在文件的底部收集其他脚注

  \[^quote]: 引用用html<q>标签替换文字“"引号字符。引用和Smartypants在语法上是不兼容的。如果两个都启用，则引用优先。注意，引用与blockquote不同，后者是标准的Markdown的一部分
  
 

[net_image]:https://imgt.388g.com/allimg/160711/5-160G10T615.jpg "net_image2"
[local_image]:https://upload-images.jianshu.io/upload_images/1768589-d4c7faea86df4437.gif "local_image2"
[jianshu_id]:https://www.jianshu.com
