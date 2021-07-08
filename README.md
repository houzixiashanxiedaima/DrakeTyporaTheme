## 介绍

<p align="left">
<img src="https://img.shields.io/badge/本人-%E9%AB%98%E7%BA%A7%E9%94%AE%E7%9B%98%E4%BE%A0-brightgreen"/>
<img src="https://img.shields.io/badge/Theme-typora-orange.svg"/>
<img src="https://img.shields.io/badge/license-Apache-blue"/>
<a href="https://jq.qq.com/?_wv=1027&k=vWsXSNBJ"><img src="https://img.shields.io/badge/QQ群-752854893-blue"/></a>
</p>


1. 本主题具备三种风格
1. 截图使用默认的字体: [JetBrains Mono](https://www.jetbrains.com/lp/mono/), 下载安装即可

1. 脚注样式来自于`维基百科`
1. 更方便的配色定制(主题组件的配色全部使用变量)
1. 推荐使用本主题制作优雅的[简历模板](https://github.com/liangjingkanji/Resume-Template), 可导出为静态网页部署[在线简历](https://liangjingkanji.github.io/Resume-Template/)



如果需要自定义字体, 请修改CSS文件`第4行`字体名称为你想要的字体即可替换全部显示字体

```css
--monospace: "JetBrains Mono", monospace;
```

- 如果第一个字体不支持中文, 则会采用第二个字体的中文, 
- 如果第一个字体未安装则会使用后续字体

## 安装方式

1. 首先确定已安装 [Typora](https://typora.io/)

2. 复制`drake.css` 到`theme`目录下然后重启, 选择菜单栏主题

3. 通过`设置 -> 外观 -> 打开主题文件夹`打开theme目录

**小标题**

```kotlin
override fun onCreate(savedInstanceState: Bundle?) {
    super.onCreate(savedInstanceState)

    state.onRefresh {
        // 一般在这里进行网络请求
        thread {
            Thread.sleep(2000)
            showContent()
        }
    }.showLoading()
}
```



使用建议

| 功能     | 建议                                                         |
| -------- | ------------------------------------------------------------ |
| 加粗     | 作者认为加粗是一种不出现在标题大纲的小标题, 原本的简单加粗效果我觉得不够明显也影响文字排版效果(建议使用代码片`代码`替代) |
| 引用     | 引用是一种警示醒目作用的文字块                               |
| 代码片段 | 代码片段是和普通文本区分的文字块, 不一定是代码               |
| 代码     | 在普通文字中一小段具备特殊含义(标记醒目)的字符串, 此文本存在背景的话作者认为影响整齐排版效果 |
| 脚注     | 对某个内容进行解释, 简短的描述建议在内容后使用()括号         |



这里演示脚注内容[^2]

> 如果对目前配色有不满的地方可以打开`.css`主题文件直接修改对应变量值, 本主题已根据语法定制好全部色值



[^2]: 脚注内容, 一般不使用脚注因为很多文档不支持`Markdown`脚注渲染(例如GitHub不支持脚注)



## 截图预览

提供多种配置预览

### drake-dark

<img src="https://raw.githubusercontent.com/liangjingkanji/DrakeTyporaTheme/master/img/thumbnail-dark.png"/>

### drake

<img src="https://raw.githubusercontent.com/liangjingkanji/DrakeTyporaTheme/master/img/thumbnail.png"/> 

### drake-light

<img src="https://raw.githubusercontent.com/liangjingkanji/DrakeTyporaTheme/master/img/thumbnail-light.png"/> 

## License

```
Copyright (C) 2018 Drake, Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

