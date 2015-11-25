
* 模拟手机点击事件

	```
	function attachEvent(src,fn){
		$(src).unbind();
		$(src).bind('touchstart',function(e){
			//...code...添加一个条件，确定我们按下开始了
		});
		$(src).bind('touchend',function(){
			//...code...判断条件是否成立，如果成立则交互
		});
		$(src).bind('touchmove',function(){
			//出现move，说明不是touch事件，需要清除start时，设置的属性
		});
	}
	//绑定事件
	attachEvent($('.list li'),function(){
		//code...
	});
	```



## 移动端触屏滑动，js事件

#### 四种touch事件

