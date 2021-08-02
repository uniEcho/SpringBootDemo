# Spring boot test
<h2>运行第一个Spring boot</h2>
<h2>springboot的控制层</h2>
<p>
  <h3>@Controller</h3>
  负责标识这个类是个Controller类，Spring检测到@Controller注解时，将其自动注册为Controller对象
</p>
<p>
  <h3>@ResponseBody</h3>
  正常情况下，Controller类中函数返回是一个模板对象（页面），但是有时候我们希望返回值数值型（字符串或者Json格式数据），这时就需要添加@ResponseBody注解
@ResponseBody注解可以添加到类或者函数上
</p>
