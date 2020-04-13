### JavaScript背景



### JavaScript组成


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

	
