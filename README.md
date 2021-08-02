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
<p>
<h3>@RequestParam</h3>
@RequestParam用于读取URL中的数据
</p>
<p>
<h3>@ModelAttribute</h3>
该注解通常在Controller上的某个方法上，此方法会首先被调用，并将方法作为Mode的属性，然后再调用对应的Controller处理方法。</p>
<p>
<h3>@RestController、@GetMapping 和@PostMapping</h3>
这三个注解都是组合注解，其中
@RestController相当于@Controller + @ResposeBody
@GetMapping相当于@RequestMapping（method=RequestMethod.GET）
@PostMapping相当于@RequestMapping（method=RequestMethod.POST）
注：@GetMapping用于获取信息（可以理解为Select操作），@PostMapping用于更新信息（可以理解为Update）。这样解释大家可能看得云里雾里，因为我们并没有明确问题的立足点：如@GetMapping是谁向谁获取信息，@PostMapping是谁发出的更新命令，这里需要明确，我们的立足点是前端（也就是前端是动作的发出者，后端是动作的执行者）。也就是：@GetMapping表示前端向后端发出请求数据命令，后端根据具体请求（URL）找到对应的资源并返回给前端。@PostMapping表示前端向后端发送数据，后端根据命令，将给数据持久化到数据库中，实现数据的更新。
</p>
<p>推荐看：https://blog.csdn.net/qq_22157917/article/details/98490976</p>
