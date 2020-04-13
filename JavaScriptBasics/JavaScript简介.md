### JavaScript背景

JavaScript出生年份：1995年（比我大一岁，哈哈哈）

出生公司：Netscape

原名：LiveScript

起初它的主要目的是处理由服务器语言负责的一些输入验证操作

### JavaScript组成

- #### ECMAScript

- #### DOM（Document Object Model 文件对象模型）

- #### BOM(Browser Object Model 浏览器对象模型)

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
		* 代码分离彻底
		* 利于后期维护
		* 不同页面之间可以复用
	* 缺点
		* 增加请求数量

	
