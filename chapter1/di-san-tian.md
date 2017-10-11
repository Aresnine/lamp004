# HTML表单

```
1、form标签：声明 标签内的内容是一个表单

2、method属性：
    1、post：密文传输，数据跟URL分开了
    2、get：通过URL进行传值，URL可见了  默认值（不写时候使用的）

3、action属性：数据提交的目标 （一个php文件）
```

## `<input type="">`：input文本输入，type决定类型

```
1、type="text"普通的文本输入框
    注意：必须有name属性

2、type="password"密码框，输入的内容不可见 name属性

3、type="email" 文本输入框  填写的内容必须为邮箱格式
    特点：1、格式必须为邮箱
          2、输入错误之后，框变色，提示用户
          3、鼠标悬停时，会有提示框

4、submit：提交
    注意：1、value值是自定义，用来显示给用户的
          2、name属性不需要

5、radio:单选框  
        特点：
        1、name必须的，有多个值的时候，name需要相同
        2、因为我们不能输入值，我们需要给一个value值

6、checkbox：复选框（多选框）
        特点：
        1、name必需的，但是name后面需要有一个[]
        2、同一组多选框的name需要相同
        3、值需要给出

7、checked：属性  表示默认选择  
        1、checked="checked"
        2、checked

8、placeholder：占位符
        特点：
        1、给用提示信息 
        2、与value的不同：
            1、他不会传送到服务器
            2、value的值改变之后，提交的值会发生改变

9、disabled：禁止使用,用户无法点击
        1、disabled
        2、disabled="disabled"

10、autofocus：光标自动聚焦
        1、autofocus
        2、autofocus="autofocus"

11、color：颜色选择框
        特点：1、传送给服务器的值是16进制

12、<select>标签：声明这是一个下拉列表
        需要<option>标签配合
        注意：
            1、name要放在select标签内
            2、value值如果给出使用value，未给出就使用所选列表项里面的值
            3、selected属性：默认选择的

13、<textarea>标签：用来输入大段的文本
        单位：不是像素
        cols：宽
        rows：高

14、url属性值：跟email类似，表示输入的文本需要是url地址
        特点：
            1、错误的时候会给出提示

15、range 滑动条
        1、默认最大值是100，最小值0
        2、max属性：最大值 min属性：最小值
        3、step属性：代表的是间距，每移动一下，所加的值

16、number属性
        1、没有默认的最大值，默认step=1
        2、商城的时候，最大值要设置 ，最小值也要设置

17、file 文件上传
        1、传输方式必须为post
        2、在form添加一个属性  enctype="multipart/form-data"

18、image 图片提交（按钮）

19、button按钮
        1、默认值  submit
        2、button 表示按钮  这时候不能提交
        3、reset  重置  清除所有输入的东西

20、hidden 隐藏 用于后期表单传值
```

其它标签：

```
1、<hr />:单标签 表示内容的变化
2、<pre> ：双标签 表示原样输出
3、iframe标签：双标签  src属性  链接的是一个html文件
```

&lt;frameset&gt;标签：框架标签

		需要&lt;frame /&gt;配合使用

		属性：

			1、rows ：表示的是横着分

			2、cols ：表示的是竖着分

		注意：不能放在body内

		frame：需要src属性，src没有的时候为空

		

		target:

			1、\_self  当前页面

			2、\_blank  新页面

			3、\_parent 父页面

