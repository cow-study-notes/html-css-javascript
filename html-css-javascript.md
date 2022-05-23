# html初学者教程
    GrandmaCan -我阿嬷都会
    初学者教程 html入門  html编程
    https://www.youtube.com/watch?v=CLUPkcLQm64

## HTML-网页骨架
    structure-结构体
## 环境建设&创建第一个网页
    1、新建一个.hmtl后缀的文件
<!DOCTYPE html> //文档类型
<html>//html开始
    <head>// 网页资讯开始
        <meta charset="UTF-8">//网页编码
        <title>新手的网站</title>//网页标题
    </head>//网页资讯结束
    <body> //网页内容开始
    hello 新手入门
    </body>//网页内容结束
</html>//html结束
    2、注解、hmtl基本标签
        <!--DIV--> 注解
        <h1> 标题
        <b> 加粗
        <i> 斜体字
        <br /> 换行
        <hr /> 分割线
    3、超链接&图片
        <a href="https://google.com/">google搜索</a>
        <img src="shuangxi.jpg" width="300" height="300"/>//本地图片
        <img src="https://www.yikaojixun.com/uploads/a05477f6aba9abbd18371290ef356ce8.jpg"/>//网络图片
    4、影片、嵌入影片
        //controls 指定必须显示音频和视频控件 
        <videos src="hejiu.mp4" controls>浏览器无法载入该视频</videos>
        //嵌入youtube视频
        <iframe width="1080" height="900" src="https://www.youtube.com/embed/CLUPkcLQm64" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    5、列表、表格
        列表：
            <ol></ol>//数字列表排序
                <ul>//列表
                    <li>Telegram</li>//内容
                    <li>facebook</li>
                    <li>googel</li>
                </ul>
        表格：
            <table>//表格
                <tr>//一行
                    <td>年</td>
                    <td>月</td>
                    <td>日</td>
                </tr>
                <tr>
                    <td>2022</td>
                    <td>05</td>
                    <td>02</td>
                </tr>
            </table>
    6、容器div、span
        <div></div>//容器-每个占一行
        <span></span>//容器-宽度多少占用多少
        <div style="color:red;"></div>//div容器里所有字体红色
    7、input输入标签
        <input type="tetx" placeholder="请输入账号"/>//输入纯文本标签，并提醒输入账号
        <input type="password" />//隐藏文本输入
        <input type="date" />//日期
        <input type="range" />//范围滑动条
        <input type="file" />//上传文件
        <input type="checkbox" />//复选框
        <textarea></textarea>//文本区域输入
    8、<meta>标签
        <meta charset="UTF-8">//网页编码
        <title>新手入门首页</title>//网页标题
        <meta name="description" content="网站简介">//网页简介
        <meta name="keyword" content="网站关键词">//网页关键词
        <meta name="viewport" content="width=device-width,initial-scale=1.0">//网页自适应大小
-
## CSS-美观和排版
    presentation-介绍/appearance-外貌
    1、如何撰写css
        内层的style属性会覆盖外层的style属性
            <div style="font-size:50px;">//字体大小（font-size）
            <h1 style="color:red;">新手css学习</h1>//字体颜色（color:red）
            <p style="background-color: rebeccapurple;">段落段落段落</p> // 背景颜色（background-color: rebeccapurple）     
            <p style="border: 5px solid black;">段落段落段落</p>//文本边框（border: 1px solid black）
            <p style="color: rgb(251, 0, 255);">段落段落段落</p>//自选颜色（color: rgb(251, 0, 255)）
    2、padding(充填) & margin(利润)
        控制div空间属性，边框可单独调控（顺时针）
        <div style="padding:20px; background-color: lightblue; border: 1px solid black;">
            新手入门学习padding & maring
        </div>
    3、float(浮动) & display(展示)
        <img src="shuangxi.jpg" width="200px" style="float: right;">//图片浮动到段落右侧（float: right;）
         <p>在很久很久以前有一群小狗，它们在不久之后就长大了！</p>
    <!--block & inline-->
        <p style="display:inline;">一块</p>//p标签一对占一行，加(display:inline;)变成对接
        <p style="display:inline;">路线</p>
        <span style="display:block;">一起</span>//span标签对接，加（display:block;）变成一对占一行
        <span style="display:block;">合体</span>
    4、position 定位
        <div style="position:fixed;"></div> //固定（position:fixed;）
        <div style="position:relative;"></div>//相对定位（position:relative;）
    5、opacity（透明度） & border-redius（边缘控制）
        <!-- opacity & border-redius-->
        <p style="position: relative; top: 65px; left: 25px;">看见我吗</p>
        <div style="opacity:0.8; border-radius:30px 20px 15px 60px; width: 120px; height: 80px; background-color: red"></div>
    6、style标签
        设置所有P标签都为红色
        <style>
        p{
            color: red;
        }
        </style>
    7、如何引入css档案
        新建一个.css文件：//
                p{
                color: red;
                }
        引入css：
            <link rel="stylesheet" href="style.css">   
    8、calss和id使用
    * 套用所有
            <h1 id="css-h1">id使用#</h1>
            <p class="txt background-grey">txt这是红色字体</p>
            <p class="txt">txt这是红色字体</p>
            <p class="rar">rar这是红色字体</p>
            <p class="rar background-grey">rar这是红色字体</p>
            css样式：
                    //calss用.连接
                        .rar{
                            color: rosybrown;
                            background-color: blueviolet;
                            }
                    //id用#连接
                        #css-h1{
                            background-color: blueviolet;
                                } 
    9、animation动画
            <h1>动画</h1>
    <div class="box box-animation"></div>
        @keyframes change-color {
    from{background-color: rebeccapurple;}
    to{background-color: brown;}

            }
            .box{
                width: 200px;
                height: 200px;
                background-color: green;
            }
            .box-animation{
                animation-name: change-color;
                animation-duration: 1s;
                animation-iteration-count: infinite;
            }

                                
## JavaScript-功能
    dynamism-活力/action-行动




