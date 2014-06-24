---
layout: page
title: Github Page (Example Code)
tagline: Just Do It!

---
{% include JB/setup %}


<div class="media">
  <a class="pull-left" href="https://github.com/examplecode/gfw_dns_resolver">
    <img class="media-object" src="/images/github.png" >
  </a>

  <div class="media-body">
   <a href="https://github.com/examplecode/gfw_dns_resolver"><h4 class="media-heading">gfw_dns_resolver</h4></a>
   <p>
    这个小工具用于获取被gfw dns 污染域名的真实ip地址，通常可以用于获取twitter,youtube,facebook等网址的真实ip地址.
  </p>
  </div>

  <a class="pull-left" href="https://github.com/examplecode/android-ui-test-runner">
    <img class="media-object" src="/images/github.png" >
  </a>
  <div class="media-body">
     <a href="https://github.com/examplecode/android-ui-test-runner"><h4 class="media-heading">android-ui-test-runner</h4></a>
    <p>
    这是一个用于android 非常简单的测试框架，帮助我们测试一些UI相关的用例,在你的TestSuite中你只需要写一个以"test"开头的方法就会自动在测试用例列表界面中展示出来，点击即可执行测试.
    </p>
  </div>

  <a class="pull-left" href="https://github.com/examplecode/gypdemo">
    <img class="media-object" src="/images/github.png" >
  </a>
   <div class="media-body">
     <a href="https://github.com/examplecode/gypdemo"><h4 class="media-heading">gypdemo</h4></a>
    <p>
      gyp 是 chromium的构建系统，这里有些小示例展示gyp如何工作。
    </p>
  </div>

</div>
<div align="right">
  
<a href="https://github.com/examplecode"> 前往Github</a>

</div>

### blogs
------------

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>


