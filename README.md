# First-play
通过js实现排他功能 日常练习

 body>
 html部分
    <input type="button" value="好人">
    <input type="button" value="好人">
    <input type="button" value="好人">
    <input type="button" value="好人">
    <input type="button" value="好人">


js部分
    <script>

    var objs=document.getElementsByTagName("input");
    // 循环遍历所有按钮
    for (var i = 0; i < objs.length; i++) {
    //    为每个按钮添加点击事件
        objs[i].onclick=function(){
        // 把所有按钮的默认值设置为好人
         for (var j = 0; j < objs.length; j++) {
           objs[j].value="好人";
         }
        //  当前被点击按钮设置为坏人
        this.value="坏人"
        }
        
    }
     
  
    </script>
</body>
