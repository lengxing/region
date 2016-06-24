# 基本功能
Region插件主要用于地域选择使用，可以同时多个地区添加

# 插件由来

由于项目功能需要，需要有一个能够多选国内市区功能的插件，
通过在网上的查找，找到了百度的[ESUI组件库](http://ecomfe.github.io/esui-family/controls/index.html)

  >ESUI is a Collection of JavaScript Controls.

但是由于ESUI内容包含广泛，而且内部依赖非常之多
（应该这套内容是百度前端“生态”中的一部分，但是维护来看截止13年就不在更新了）
所以在ESUI的基础上面，将地域选择的功能进行了摘取。
从而，有了次Rep的出现。

  由于目前的项目需要，所以只是摘取了多选功能部分，其他部分功能暂时没有进行完善。
  后续会尽可能的不断完善。

# 使用说明

![Example](/images/example_1.png)

  HTML:

  	<div id="region_test" class="ui-ctrl ui-region"></div>

  Javascript:

  	<script>
        $(function () {
            var options = {
                main: "#region_test",
                value: '268,25,10,778'
            }
            var region = new Region(options);
        })
    </script>

  依赖：

  	- jquery.js
  	- underscore.js

  接口方法：

  	- getRawValue 获取选择区域的数组值