 html winow弹窗案例
html_learning

- 实现过程
  1，创建一个页面
      ** 有两个输入项和一个按钮
      ** 按钮上面有一个事件：弹出一个新窗口  open
  2， 创建弹出页面
      ** 表格
      ** 每一行有一个按钮和编号的姓名
      ** 按钮上有一个事件： 把当前的编号和姓名，赋值到第一个页面的相应的位置
      
      ****// 实现s1方法
          function s1(num,name){
                //需要把num和name赋值到window页面
                //跨页面的操作  opener：得到创建这个窗口的窗口 得到window页面
                var pwin = window.opener;
                pwin.document.getElementById("numid").value = num;
                pwin.document.getElementById("nameid").value = name;
                //关闭窗口
                window.close();
      }
      
     
