# 每天一练————表单

标签（空格分隔）： HTML

---说明：介于本人对表单的不熟悉，故通过此方法来加强，有什么不妥之处， 请多多指教！若有对web前段感兴趣，并未来从事此行业的，可以与我联系，交流交流经验与技术。QQ：573972520

## 表单的定义 ##

表单是一个包含表单元素的区域。 表单元素是允许用户在表单中（比如：文本域、下拉列表、单选框、复选框等等）输入信息的元素。
并且表单使用`<form>`标签来进行定义。

        <form>
             /*输入内容 input 元素*/
        </form>   

## 输入 ##

 - 1.文本域
    当你需要在网页的表单中输入文字或者数字的时候，便会使用到文本域
代码如下所示：

         <form>
    		用户名：
     		<input type="text" value=""/>
    		<br />
    		密码：
    		<input type="password" value="" />
          </form>


从上面的代码我们可以知道，可以通过`<input>`标签来进行输入，并且通过`<type>`来指定输入的类型，在用户名那里是文本类型`text`，在密码那里是`password`,接着我们发现还有另外一个值，那就是`<value>`，我通过实验明白这一`<value>`标签是可以在你的输入框里提前定制内容的。比如你在`<value>`后面输入K，那么在你的用户名的输入框里就出现了一个K，在密码的输入框里就出现了一个小圆圈。（因为密码不能看见具体的数字和字母嘛O(∩_∩)O）


----------

 - 2.单选按钮 
接下来我进行了单选按钮的测试，先看代码

         <form>
		    <input type="radio" name="hot" value=""  />hot
	      	<input type="radio" name="hot" value="" />cool
	     </form>
	 
单选按钮的`type`是`radio`类型的并且多了一个`name`属性，这一属性很关键，细心的同学都发现了两个`name`都是一样的，在这里如果二个`name`不相同，那么它们就不能实现单选的效果，而是实现了多选的效果，所有一定要记得要想要实现单选效果`name`要一致哦！


----------

 - 3.复选效果
 复选效果可以选择多个选项，代码如下

          <form>
			<input type="checkbox" name="checkbox" value=""/>香蕉
			<input type="checkbox" name="checkbox" value="" />苹果
			<input type="checkbox" name="checkbox" value="" />橘子
		  </form>

复选按钮的`type`是`checkbox`类型哦。


----------

 - 4.文本域
 文本域就是可以让用户在文本域中输入文字。代码如下

    	<textarea name="" rows="10" cols="10">please input you advice </textarea>
    	
在这里新增了一些新的代码如`rows`与`cols`。
`rows`属性规定 textarea 的可见高度。`cols` 属性规定 textarea 的可见宽度.
在这里我发现不同的浏览器有不同效果，在Chrome和Firefox中它们呈现的文本域是可以拉伸的，但是在Edge和IE中就就不能拉伸。


----------

 - 5，选择列表
选择列表代码

     	<select name="select" value="choose">
			<option value="A">香蕉</option>
			<option value="B">苹果</option>
			<option value="V">橘子</option>
		</select>

通过`<select>`进行创建，在`<option>`中填写你需要的列表内容。
	

    

    




