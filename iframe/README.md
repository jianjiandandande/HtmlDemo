# html框架

## frameset框架集
   >创建框架网页的步骤：
      1.创建各个子窗口对应的html文件
      2.创建整个框架文件，分别引用子窗口文件
      
    >创建框架页面的基本语法：
    
      * frameset就是用于将窗口划分成不同模块
      * cols纵向划分
      * rows横向划分
          ** cols与rows的划分：
            pixels--具体的宽度
            % --占浏览器的百分数
            * --剩余宽度
      * border边框的粗细
      * frame 框架标签,网页被划分成几个部分，就会有几个freme,里边的src是用来引用已经设计好的子窗口的网页文件
      **注意：<frameset></frameset>标签不能与<body></body>标签同时使用。除非你在<frameset>中使用<noframe>标签，此时<body>标签可以嵌套在<noframe>标签中**
      ```
      <frameset cols = "25%,50%,*" rows="50%,*" border="5">
        <frame src = "top.html">

        ......

      </frameset>
      ```
## iframe内嵌框架
   > iframe比较灵活，它可以嵌套在网页的任一个指定的位置。比较灵活
    属性(括号中为属性的取值)：
    
      * frameborder(0、1)规定是否显示框架周围的边框
      * name (frame_name)规定iframe的名称
      * scrolling (yes、no、auto)规定是否在iframe中显示滚动条
      * src(URL)规定在iframe中显示的文档的URL

    **iframe属于网页内容的一部分，它放置在<body></body>当中**
    
