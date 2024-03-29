<a name="1">顶部 </a>

### 分级标题('#')
\#+空格+一级标题  
# 一级标题  
\##+空格+二级标题  
## 二级标题  
\###+空格+三级标题  
### 三级标题  
\####+空格+四级标题  
#### 四级标题  
\#####+空格+五级标题  
##### 五级标题  
\######+空格+六级标题  
###### 六级标题  

---
### 空格(' ')
1空格 = N空格/1换行 建议：1空格  
N空格 = 多个\&ensp;
```html
<pre>标签
&ensp; 半方大的空白
&emsp; 全方大的空白
&nbsp; 不断行的空白格
```
---
### 换行(' '+'回车')  
1换行 = 2空格+1换行 建议：2空格+1换行  
2换行 = 2换行 建议：2换行  
N换行 = 多个\<br>

---
### 强调(*_~)
\*斜体* 或者 \_斜体_  
*斜体*，_斜体_  

\*\*粗体** 或者 \_\_粗体__  
**粗体**，__粗体__  

\*\*\*加粗斜体***  
***加粗斜体***  

\~\~删除线~~  
~~删除线~~

---
### 区块引用(>)
> 一一一一一一一一一一    
二二二二二二二二二二   
三三三三三三三三三三  

> 四四四四四四四四四四  
五五五五五五五五五五  
>> 六六六六六六六六六六  
七七七七七七七七七七  
八八八八八八八八八八  
>>> 九九九九九九九九九九   
十十十十十十十十十十  

---
### 代码区块(tab)
\`\`\` javascript
``` javascript
	void main()
	{
		printf("Hello, Markdown.");
	}
	#include <stdio.h>
```
\`\`\`

---
### \<pre>

<pre>
├── build                        // webpack配置目录
│   ├── utils.js     		         // 工具文件
│   ├── config.js     		       // 配置文件
│   ├── webpack.config.base.js   // 基础构建
│   ├── webpack.config.dev.js    // 开发模式构建
│   ├── webpack.config.prod.js   // 生产模式构建
├── dist               		       // 生产目录
├── src                		       // 开发目录
├── .babelrc                		 // babel配置
├── .editorconfig                // editorconfig配置
├── .eslintignore                // eslint排除的检测范围
├── .eslintrc.js                 // eslint配置
├── postcss.config.js            // postcss配置
</pre>  

---
### 无序列表(-/+/* 加空格)
- 第一项  
- 第二项
+ 第一项
+ 第二项
* 第一项
* 第二项

---
### 有序列表('1. 加空格')
1. 第一项  
2. 第二项

---
### 表格('|-')
学号\|姓名\|分数  
-|-|-  
小明\|男\|75  
小红\|女\|79  
小陆\|男\|92  

学号|姓名|分数
-|-|-
小明|男|75
小红|女|79
小陆|男|92

---
### 分割线
***
---
___
\*** --- ___

---
### 文字连接('\[\]\(\)')
欢迎来到[baidu-停留没提示](http://baidu.com)
欢迎来到[baidu-停留有提示](http://baidu.com "baidu")

---
### 图片链接('\!\[\]\(\)')
![美丽花儿](http://ww2.sinaimg.cn/large/56d258bdjw1eugeubg8ujj21kw16odn6.jpg "美丽花儿")

---
### 自动链接('<>')
<http://example.com/>  
\<http://example.com/>

---
### 锚点
<a href="#1">回到顶部</a>  
\<a href="#1"\>回到顶部\</a\>

---
### 内容目录
在段落中填写 [TOC] 以显示全文内容的目录结构。

---
### 反转义作用(\)
\!\[图片名称]\(图片地址)  
\>>反转义作用  
\***  
\- 变成普通符号  

---
### 标记作用 (``)
`ctrl+a`

---
### Fork或借鉴请注明出处 [@ HeavenBin](https://github.com/HeavenBin/MarkdownCourse)
