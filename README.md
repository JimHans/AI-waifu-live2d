# AI-waifu AI加持的网页看板娘

    く__,.ヘヽ.　　　　/　,ー､ 〉
    　　　　　＼ ', !-─‐-i　/　/´        ver.   || |
    　　　 　 ／｀ｰ'　　　 L/／｀ヽ､            | | ||         Live2D 看板娘 AI Version 前端&后端API封装
    　　 　 /　 ／,　 /|　 ,　 ,　　　 ',     ||||| |||        Version 1.0.7 (Based on FGHRSH Version V1.4.2)
    　　　ｲ 　/ /-‐/　ｉ　L_ ﾊ ヽ!　 i      ||    | ||||       Update 2020-08-19 Modified By JimHan From the FGHRSH Version
    　　　 ﾚ ﾍ 7ｲ｀ﾄ　 ﾚ'ｧ-ﾄ､!ハ|　 |
    　　　　 !,/7 '0'　　 ´0iソ| 　 |                           1.1.5版本基于FGHRSH V1.4.2版本魔改
    　　　　 |.从"　　_　　 ,,,, / |./ 　 |                     原版地址https://github.com/fghrsh/live2d_demo 具体食用方法参照原版
    　　　　 ﾚ'| i＞.､,,__　_,.イ / 　.i 　|                    更新日期2020-08-19，若要使用自建NLP请参照下方“使用腾讯云NLP服务自建NLP服务”
    　　　　　 ﾚ'| | / k_７_/ﾚ'ヽ,　ﾊ.　|
    　　　　　　 | |/i 〈|/　 i　,.ﾍ |　i　|        Thanks
    　　　　　　.|/ /　ｉ： 　 ﾍ!　　＼　|          journey-ad / https://github.com/journey-ad/live2d_src
    　　　 　 　 kヽ>､ﾊ 　 _,.ﾍ､ 　 /､!             xiazeyu / https://github.com/xiazeyu/live2d-widget.js
    　　　　　　 !'〈//｀Ｔ´', ＼ ｀'7'ｰr'          Live2d Cubism SDK WebGL 2.1 Project & All model authors.
    　　　　　　 ﾚ'ヽL__|___i,___,ンﾚ|ノ
    　　　　　 　　　ﾄ-,/　|___./
    　　　　　 　　　'ｰ'　　!_,.:

### 1.1.5版本更新：
- 新增了动态的交互窗口，使主题更契合
- 修复了工具栏在桌面方式下无法点击的问题，并优化工具栏配色   
- 优化工具栏图标
- API新增更多形象（基于https://xiaoyou66.com/ 提供的API）
- 修复了杂七杂八的Bug

## 目录结构
```
│  demo1-default.html       // 常规引用 Demo
|  relax.html               // 休息提醒页面
│
└─assets
        autoload.js                     // 自动异步加载
        flat-ui-icons-regular.eot       // Flat UI 字体
        flat-ui-icons-regular.svg       // Flat UI 字体
        flat-ui-icons-regular.ttf       // Flat UI 字体
        flat-ui-icons-regular.woff      // Flat UI 字体
        jquery-ui.js                    // 自带的jQuery UI库
        jquert.min.js                   // 自带的jQuery核心库
        live2d.js                       // Live2D 核心
        waifu-tips.js                   // Live2D 看板娘 核心脚本
        waifu-tips.json                 // Live2D 看板娘 提示语
        waifu.css                       // Live2D 看板娘 CSS样式表
```

### 食用方法与@fghrsh的修改版本相同

## 扩展功能：使用腾讯云NLP服务自建看板娘的NLP服务
- 此版本本身拥有默认的NLP服务，但在此仍建议你使用自建NLP。注意，自建NLP需要你拥有腾讯云账号并经过实名验证。其它厂商的API暂时不被支持。
- 自建NLP方式如下：
#### 1.在腾讯云官方网站https://cloud.tencent.com/ ，点击产品->人工智能->自然语言处理，再点击免费体验，按提示开通NLP免费服务。
#### 2.点击右上角个人头像->访问管理->访问密钥->API密钥管理，新建一个密钥。注意！为了保障你的账号安全，建议使用子账号创建密钥。具体创建方法详见腾讯云官方最佳实践文档https://cloud.tencent.com/document/product/598/10592 。
#### 3.创建密钥后，妥善保管你的密钥，切换回自然语言处理的控制台页面，点击管理中心->快速使用->打开工具，选择闲聊板块，代码语言为PHP，将你的密钥按要求填入后，按照你的要求调节参数，最后，将生成的代码复制，粘贴入新的文本文档，保存为xx（你自己的名字）.php，并放入你服务器的自定义目录。
#### 4.在AI看板娘配置文件waifu-tips.js中，找到并修改NLP模块的API调用地址为你新建的php文档的URL。
#### 5.在https://getcomposer.org/ 页面，或者按照其它教程安装composer插件，并将生成的vender文件夹移至xx.php的同一目录下。
#### 6.到此处，你的AI看板娘API应该就可以运行了。如果有其他问题，可以查找腾讯云文档解决，或者检查你的composer插件是否安装正确。当然，如果出现403等问题，你也要检查一下文件的权限问题。


## 感谢以下项目
[live2d_demo / ©fghrsh / GPL v2.0][1]  
[live2d-widget / ©xiazeyu / GPL v2.0][2]  
[live2d_src / ©journey-ad / GPL v2.0][3] 

- Live2d Cubism SDK WebGL 2.1 Project & All model authors.

Open sourced under the GPL v2.0 license.


  [1]: https://github.com/fghrsh/live2d_demo
  [2]: https://github.com/xiazeyu/live2d-widget.js
  [3]: https://github.com/journey-ad/live2d_src
