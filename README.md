#EDM 邮件营销的html&css 点滴
最近公司每个月都会制作公司的Newsletter，发送给客户做edm营销。记得第一家公司每周都会做edm，也是自己工作的一个重要部分。做的当中会发现有很多坑，很多css属性不支持，各个邮件服务器的显示上也会存在很多的差异，所以在这里把这些记录下来

###如何制作edm

```css
body { margin: 0; padding: 0;}
    table.Newsletter {font: 12px/18px arial; color: #4b4b4b }
    table.Newsletter a { text-decoration: none; }
    table.Newsletter a:hover { color: #bd2d34; text-decoration: underline;}
    table.Newsletter img{display: block}
