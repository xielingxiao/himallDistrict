# himallDistrict
四级地区选择插件，商品详情选择送货地址

目前四级地址库均通过接口传递父级id，返回子级地址对象，也可以使用本地地址库（这里已附上本地地址库json，大小122KB），修改插件中子级getData获取的地方即可；

参数配置：

var defaults = {
			id : $(this).attr("id"),// 设置id
      
			renderTo : $(this).parent(),// 指定绑定源
      
			items : new Array(),// 地区数据源
      
			select : '',// 默认选中项,优先从this的data-select属性获取默认选中值
      
			ajaxUrl:'',
      
			closeFn : function() {}// 关闭时回调};
      
      
示例如下：

