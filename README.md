# test

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

# vue项目第一个CLI工程案例
以下为vue官网文档学习内容：
1.安装<br>
2.介绍<br>
3.vue实例<br>
4.语法模板<br><hr>
5.计算属性和监听器<br>
-   计算属性：相当于是依赖于vue实例的属性的属性，比如vue属性有firstname和lastname，那么fullname就可以作为一个计算属性存在于实例中。
-   计算属性可以理解为对vue实例属性进行某些计算或者处理而得到的属性
-   计算属性基于缓存机制，同样是对原有属性进行操作得到的属性，它比函数、或者vue.$watch事件监听更简洁，效率更高
-   计算属性可以添加get和set方法，详见官方文档"计算属性和侦听器"-"计算属性的setter"章节
-   侦听器用在什么时候？计算属性其实很高效很方便了，当需要在数据变化时候执行异步操作、开销非常大的操作的时候，需要监听器、监听事件。官方提供了一个$watch异步事件案例
<br><hr>
6.Class属性绑定、内联Style绑定<br>
div v-bind:class="[{ active: isActive }, errorClass]" /div   isActive是bool变量，为真时active被作用为class，errorClass总是被作用为class。这就是Class绑定Style的数组语法和对象语法；作用在自定义组件上的时候用法是相同的，这一部分可详见官方笔记；<br>
绑定内联style: div v-bind:style="{ color: activeColor, fontSize: fontSize + 'px' }" /div  其中的activeColor和fontSize是vue的变量,语句是css语句<br>
最好的方法是直接为v-bind:style="style对象变量"，比如: div v-bind:style="styleObject" /div   <br>
在vue实例中:<br>
data: {<br>
  styleObject: {<br>
    color: 'red',<br>
    fontSize: '13px'<br>
  }<br>
}<br>
<hr>

7.条件渲染<br>
v-if/v-else，常用方法是将需要根据变量的bool值决定是否渲染的那些DOM添加到一个template标签里: template v-if="bool变量名" <br>
<br><hr>

8.列表渲染<br>
v-for,还有很多其他用法，详见官方文档<br><hr>

9.事件处理<br>
v-on 相当于@，可以用内联函数语句，也可以指定调用的函数名<br><hr>

10.表单输入<br>
v-model<br><hr>

11.


