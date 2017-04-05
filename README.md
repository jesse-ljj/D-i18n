## D-i18n

后处理翻译

### DONE

* 基本翻译
* Map表维护
* 开发体验的提升(编译时开发的时候有实时替代功能，但是在一些没有集成`webpack`或`gulp`等构建工具的情况，如何进行实时的翻译) 

### TODOS
 
* env环境的区别
* 动态翻译函数(通过全局注入一个翻译函数), 静态翻译函数(编译阶段直接进行文案的替换)
* 单/复数(pipe符号去识别)
* 国际化图片(同样通过在路径上进行标识,最后输出对应的语言版本的图片路径)  运行时,自身进行标明图片路径(提供了数据双向绑定的framework) 了解framework完成数据双向绑定的原理 或使用构建工具进行替换data-locale-src='/static/img/${locale}/file.png'(基于文本的处理,那如何去找到上下文?)
* 样式表的处理(通过在class上进行标记,最后输出相对应的语言版本的class)  运行时，自身进行class进行标明(提供了数据双向绑定的framework)  或使用构建工具进行替换data-locale-class="${locale}"
* NPM包
* 弄明白vue框架的编译过程，然后添加动态翻译功能. 翻译函数(全局?), 模板上的静态文案编译的时候即完成翻译

### 技术方案梳理

`webpack`构建工具编译过程中, 抽取`map`表


### Some Tips

* `live reload`和`hot reload`的区别
