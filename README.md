#EDM Template
>最近公司每个月都会制作公司的Newsletter，发送给客户做edm营销。记得第一家公司每周都会做edm，也是自己工作的一个重要部分。做的当中会发现有很多坑，很多css属性不支持，各个邮件服务器的显示上也会存在很多的差异，所以在这里把这些记录下来

> [12 Killer Tips and Tricks for Building HTML Email](http://www.queness.com/post/8784/12-killer-tips-and-tricks-for-building-html-email)
###html 设计规范
1. 宽度保持在600到800px范围
2. html布局请使用表格布局，居中排版
    ```html
    <table width="100%" cellpadding="0" cellspacing="0" border="0">
        <tbody>
          <tr>
            <td>
              <table width="750" align="center" cellpadding="0" cellspacing="0" border="0">
                <tbody>
                    <tr>
                        <td>EDM 内容区域</td>
                    </tr>
                </tbody>
              </table>
            </td>
          </tr>
        </tbody>
    </table>
    ```
    [demo](http://jsfiddle.net/vincehu/8mez2ztt/)       
    
4. html使用`utf-8`编码
4. html代码中不能包含`JavaScript` 和 `Flash`     
5. 设计时尽量做到简洁，不适用背景图片，需要背景图片的地方使用背景颜色，或者通过css控制，在支持css 背景图片的客户端中显示背景图片，不支持的时候显示纯色的背景颜色
6. 使用table布局页面
7. 必须用`<a>`添加链接，不要使用热点`<map>`
8. `body`中不要设定背景色，不然在转发邮件的时候，转发人写的信息背景色都会变为被转发邮件的背景色，影响浏览。如果一定要给邮件模板设定整体背景色，请在模板文件最外面加一个`table`，设定此`table`的背景色

###css 设计规范
1. 所有css必须写在元素标记内，且不能使用用于布局的css属性：display、position、float
2. 这是很重要的，不是所有的CSS属性的支持。在电子邮件客户端CSS的支持是有限的，不如IE6。例如，背景图像不被前景2007/10支持时，Windows Live Hotmail和Gmail。所以，你需要知道什么是支持的。下面的链接是通过reputatable在线电子邮件管理服务编译的CSS支持广泛的名单 - 运动监视器。这个CSS列表经常更新。       
[CSS列表](https://www.campaignmonitor.com/css/)
