# GRE-CN
中文主导的GRE备考资料

[Old English README](README-EN.md)

## 关于
这个项目里的文件是大多数我个人需要的GRE备考资料，我尝试用程序转制了大部分的文件，让它们看起来更干净、可读、Git(-LFS)友好。

**因为这个项目是根据我自己的学习进度的，所以我会逐渐地补充文件。我希望在我自己考完GRE之后这个项目能涵盖GRE所需的大多数资料并帮到更多的人。**
  
目前我个人的进度呢:

- [x] 单词
- [ ] 其他待续

## 文章列表

## 文件列表
DOS下`tree /F`命令的输出:

```
C:\Code\Documents\GRE-CN (master -> origin)
λ tree /F
文件夹 PATH 列表
卷序列号为 5E78-D96D
C:.
│  .gitattributes
│  LICENSE
│  README-EN.md
│  README.md
│  TreeToPaste.bat
│  
└─L-GRE-词汇
    ├─L-GRE-Magoosh
    │      L-GRE-MagooshFlashcard.csv
    │      L-GRE-MagooshFlashcard.xlsx
    │      
    ├─L-GRE-Pre2012
    │  ├─L-GRE-杨鹏17天搞定GRE单词
    │  │      L-GRE-17天搞定GRE单词完全版-杨鹏.pdf
    │  │      
    │  ├─L-GRE-词以类记
    │  │      L-GRE-GRE词以类记-张红岩.csv
    │  │      L-GRE-GRE词以类记-张红岩.xls
    │  │      
    │  ├─L-GRE-词汇精选9th
    │  │      L-GRE-词汇精选9th.csv
    │  │      L-GRE-词汇精选9th.pdf
    │  │      L-GRE-词汇精选9th.xls
    │  │      
    │  └─L-GRE-陈琦3000
    │          L-GRE-陈琦新GRE核心3000词大愚整理版.csv
    │          L-GRE-陈琦新GRE核心3000词大愚整理版.xls
    │          
    ├─L-GRE-佛脚词汇
    │  ├─L-GRE-佛脚词汇
    │  │      L-GRE-佛脚词表.csv
    │  │      L-GRE-佛脚词表.xlsx
    │  │      
    │  └─L-GRE-佛脚词汇网络版2017
    │          GRE佛脚词汇表网络版2017.pdf
    │          
    ├─L-GRE-再要你命3000
    │  ├─L-GRE-3000词助记与精炼
    │  │      L-GRE-GRE核心词汇助记与精练第2版.pdf
    │  │      
    │  ├─L-GRE-再要你命3000顺序版
    │  │      L-GRE-再要你命3000.csv
    │  │      L-GRE-再要你命3000.xlsx
    │  │      
    │  └─L-GRE-再要你命3000顺序版QA
    │          L-GRE-再要你命3000顺序版QA.txt
    │          
    ├─L-GRE-巴朗词表
    │      L-GRE-Barron3500.pdf
    │      
    └─L-GRE-机经词汇
        └─L-GRE-机经词汇-霍
                COPYING
                L-GRE-同义词乱序-霍.CSV
                L-GRE-机经词汇-霍.CSV
                L-GRE-机经词汇-霍.xlsx
                L-GRE-补充词汇-霍.CSV
```

## 技术方面
#### PDF --> CSV
写了一个自动识别PDF中的表格，并且把连续的表格拼起来，再转成Excel格式的程序(闭源))。得到的xlsx文件再经过Microsoft Excel 2016导出为在线可读的csv。

#### PDF --> Searchable PDF
同样是一个轮子(闭源)，对于非表格的PDF文件全文件调用Keras以及预先训练好的中英文字符识别数据集，通过机器学习识别文件中的文字并且在PDF上加一层可搜索的文字层。

## 命名规则
这个项目里的文件都是以`"L-" + "GRE-" + "Subject-" + "Source" + ".Extension"`方式命名的，主要是由于我个人电脑上的命名方式比较特殊，而这个仓库是通过一个同步程序自动导出并上传我的指定文件的。

## 贡献
没什么好贡献的。不过如果您有推荐的资料或者文件，请开个Issue告知一下，我会考虑加到repo里。

## 协议
文本文件、代码 (CSV, Python, Go, TXT文件) 以BSD-3-Clause协议开源  
PDF和Office文档，除非额外说明协议，否则均以CC-BY-NC-ND国际许可协议共享  
音视频文件基本不是原创，所以版权均归原作者所有