项目说明：
    参考资料：
    1、《Jasmine单元测试框架使用基本介绍》 链接：https://segmentfault.com/a/1190000005954868
    2、《正则表达式30分钟入门教程》链接：http://www.jb51.net/tools/zhengze.html
    
    重要测试功能说明
    A:本测试是在IntelliJ IDEA环境进行的。
    第一部分：RSS Feeds 
               
                1.var regularExpressionUrl = /^((ht|f)tps?):\/\/([\w\-]+(\.[\w\-]+)*\/)*[\w\-]+(\.[\w\-]+)*\/?(\?([\w\-\.,@?^=%&:\/~\+#]*)+)?/;检查 URL 格式是否正确的正规表达式，根据审核意见， 查看了参考资料2的内容
                2.遍历所有数组，判断数组的方法，参考了资料1的方法来做。
     
     第二部分：The menu
     
                1.打开首页点解Icon，查看html代码发现隐藏/展开菜单是根据css类.menu-hidden和.slide-menu实现的，以此做判断
                2.首先判断页面中是否含有.menu-hidden,然后用trigger方法设置点击一次，判断.menu-hidden是否消失，再点击一次，判断.menu-hidden是否出现。
                             
     第三部分：Initial Entries
                利用beforeEach和done（）
      
      第四部分：New Feed Selection
                分别加载了loadFeed（1，done）和loadFeed（2，done），存储在变量beforloads和afterloads，用方法tobe判断，参考了资料1：toEqual()：相当于==，注意与toBe()的区别。
                一个新建的Object不是（not to be）另一个新建的Object，但是它们是相等（to equal）的。
                toBe()：相当于===比较。
      