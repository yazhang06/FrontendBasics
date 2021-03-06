### JavaScript背景

JavaScript出生年份：1995年（比我大一岁，哈哈哈）

出生公司：Netscape

原名：LiveScript

起初它的主要目的是处理由服务器语言负责的一些输入验证操作

### JavaScript组成

- #### ECMAScript

  - 由ECMA-262定义，提供核心语言功能

- #### DOM（Document Object Model 文件对象模型）

  - 是针对XML但经过扩展用于HTML的应用程序编程接口，DOM把整个页面映射为一个多层节点结构
  - 提供访问和操作网页内容的方法和接口
  - DOM级别：
    - DOM1: 
      - DOM核心： 如何映射基于XML的文档结构
      - DOM HTML： 在DOM核心的基础上进行扩展，添加了针对HTML的对象和方法
    - DOM2: 在原来的DOM的基础上扩充
      - DOM视图（DOM Views）：定义了跟踪不同文档
      - DOM事件（DOM Events）：定义了事件和事件处理的接口
      - DOM样式（DOM Style）：定义了基于CSS为元素应用样式的接口
      - DOM遍历和范围（DOM Traversal and Range）：定义了遍历和操作文档树的接口
    - DOM3 ： 引入了以统一方式加载和保存的文档方法

- #### BOM(Browser Object Model 浏览器对象模型)

  - 提供与浏览器交互的方法和接口

### JavaScript位置

* #### 行间JS
  
	```
	<div onclick="alert(11111111)"></div>
  ```
	
	* 优点
		* 直接作用于当前元素
	* 缺点
		* 无法复用
		* 结构不清晰（JS,CSS,HTML混在一起）
	
* #### 内部JS
	```
	<script>
		//这里是js代码
	</script>
	```
	* 优点
		* 代码分离清晰
		* 较利于后期修改维护
		* 同页面可以复用
	* 缺点
		* 不同页面无法复用
		* 不同页面修改维护较麻烦
	
* #### 外部JS

    ```
    <script src="main.js"></script>
    ```
    * 优点
    	
    	代码分离彻底
    	
    	利于后期维护
    	
    	不同页面之间可以复用
    * 缺点
    	
    	* 增加请求数量

- ####  script放置位置

  - 放在head里（⚠️不推荐使用！！！）
    - 页面读到body标签的时候开始解析页面，当页面结构未生成的时候，在head标签中的js代码如果获取元素，将获取失败
    - 解决办法：将需要获取元素的方法放在window.onload（等待窗口加载）事件中
  - 放在body结束标签前，让HTML结构先行加载完成

- #### <script> 标签属性

  - async：可选。表示应该立即下载脚本，但不妨碍页面中的其他操作。只对外部脚本文件有效。
  - charset：可选。表示通过src属性指定的代码的字符集（大多数浏览器忽略这个属性的值）
  - defer: 可选。表示脚本可以延迟到文档完全被解析和显示之后再执行。只对外部脚本文件有效
  - language：已废弃
  - src: 可选。表示包含要执行代码的外部文件
  - type：必选。表示编写代码使用的脚本语言内容类型。默认值为text/javascript





