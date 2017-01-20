# Lazy Load Plugin for jQuery

Lazy Load delays loading of images in long web pages.
�������ӳ��˳�ҳ�������ͼƬչʾ��
Images outside of viewport wont be loaded before user scrolls to them.
���Ӵ���֮���ͼƬһ������û����������ǵ�λ��֮ǰ�ͼ�����ЩͼƬ��
This is opposite of image preloading.
�����ͼƬ��Ԥ���ء�

Using Lazy Load on long web pages containing many large images makes the page load faster.
��һ�����ݺܶಢ�Ҵ��д���ͼƬ��ҳ���У�ʹ�������ػ���ҳ����صĸ��졣
Browser will be in ready state after loading visible images.
�����������е�ͼƬ�������֮��Ž���ready״̬��
In some cases it can also help to reduce server load.
��ĳЩ�������Ҳ�ܰ������ٷ���˸��ء�
Lazy Load is inspired by [YUI ImageLoader](http://developer.yahoo.com/yui/imageloader/) Utility by Matt Mlinac.

## How to Use?

Lazy Load depends on jQuery. Include them both in end of your HTML code:
����������jQuery���������������ļ��ŵ����HTML���������

```
<script src="jquery.js" type="text/javascript"></script>
<script src="jquery.lazyload.js" type="text/javascript"></script>
```

You must alter your HTML code. URL of the real image must be put into data-original attribute.
������޸����HTML���롣������ͼƬURL����ŵ�data-original�����С�
It is good idea to give Lazy Loaded image a specific class.
����Ҫ�����ص�ͼƬһ�������class��һ���ܺõ��뷨��
This way you can easily control which images plugin is binded to.
ͨ�����ַ�ʽ����������ɵĿ�����ЩͼƬ����Ҫ���������ء�
Note that you should have width and height attributes in your image tag.
��Ҫע����ǣ�����Ҫ�����image��ǩ������width��height���������ԡ�
```
<img class="lazy" data-original="img/example.jpg" width="640" height="480">
```

then in your code do:
Ȼ�������js����������Ҫ��ô����
```
$("img.lazy").lazyload();
```

This causes all images of class lazy to be lazy loaded.
��������ʵ�����д���lazy��ʽ��ͼƬ���������ˡ�
More information on [Lazy Load](http://www.appelsiini.net/projects/lazyload) project page.

## Install

You can install with [bower](http://bower.io/) or [npm](https://www.npmjs.com/).


```
$ bower install jquery.lazyload
$ npm install jquery-lazyload
```


# License

All code licensed under the [MIT License](http://www.opensource.org/licenses/mit-license.php). All images licensed under [Creative Commons Attribution 3.0 Unported License](http://creativecommons.org/licenses/by/3.0/deed.en_US). In other words you are basically free to do whatever you want. Just don't remove my name from the source.

