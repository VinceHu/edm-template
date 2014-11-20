#EDM Template
>最近公司每个月都会制作公司的Newsletter，发送给客户做edm营销。记得第一家公司每周都会做edm，也是自己工作的一个重要部分。做的当中会发现有很多坑，很多css属性不支持，各个邮件服务器的显示上也会存在很多的差异，所以在这里把这些记录下来

###edm html设计规范
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

3. html使用`utf—8` 编码
4. html代码中不能包含`JavaScript` 和 `Flash`        
5. 设计时尽量做到简洁，不适用背景图片，需要背景图片的地方使用背景颜色，或者通过css控制，在支持css 背景图片的客户端中显示背景图片，不支持的时候显示纯色的背景颜色
