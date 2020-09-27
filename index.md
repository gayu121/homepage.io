<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>个人主页</title>
    <script type="text/javascript">
        var currentTime = new Date(); //获取Date对象的一个实例
        var hour = currentTime.getHours(); //获取小时数
        var minu = currentTime.getMinutes(); //获取分钟数
        alert("您好！现在是" + hour + ":" + minu + "\r高宇的个人主页！"); //弹出提示对话框

        function realSysTime(){
            var now=new Date();			//创建Date对象
            var year=now.getFullYear();	//获取年份
            var month=now.getMonth();	//获取月份
            var date=now.getDate();		//获取日期
            var day=now.getDay();		//获取星期
            var hour=now.getHours();	//获取小时
            var minu=now.getMinutes();	//获取分钟
            var sec=now.getSeconds();	//获取秒钟
            month=month+1;
            var arr_week=new Array("星期日","星期一","星期二","星期三","星期四","星期五","星期六");
            var week=arr_week[day];		//获取中文的星期
            var time=year+"年"+month+"月"+date+"日 "+week+" "+hour+":"+minu+":"+sec;	//组合系统时间
            clock.innerHTML="当前时间："+time;	//显示系统时间
        }
        window.onload=function(){
            //window.setInterval(realSysTime,1000);	//实时获取并显示系统时间
            window.setInterval("realSysTime()",1000);	//实时获取并显示系统时间
        }
    </script>

    <link href="css/boke.css" rel="stylesheet">


</head>
<body>
<header>
    <div class="head" >

        <h1 class="logo">gy的博客</h1>

        <li><a href="index.html" target="_parent">网站首页</a> </li>

        <li ><a href="about.html" target="_parent">关于我</a> </li>
        <li><a href="inform.html">填写个人信息</a></li>
        <li><a href="update.html">修改密码</a></li>
        <li><a href="liuyan.html">留言</a></li>

    </div >

</header>

    <div class="body">
        <img src="image/banner02.jpg" alt="">
    </div>
    <div  id="clock" class="a2"></div>
    <div class="a1" >
        <img src="image/zd02.jpg" alt=""><br><br><br>


        昵称：<a href="index.html">gy的博客</a><br>
        加入时间：2019.2.21 <br>
        粉丝：<a href="#">5</a> <br>
        关注：<a href="#">6</a>  <br>

    </div>






</body>
</html>
