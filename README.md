# Ideas
Some ideas to code


# List

## Research

## Log/Trace
log和trace本质上是相同的，把两者放在一起考虑，把现有的工作理出一个体系出来  
从研究对象、研究场景、研究目标等方面考虑  
研究对象从最简单的log，到execution trace，再到end-to-end trace  
研究场景从只有log（大部分日志分析系统面临的是只有log），到除了log还有可执行文件，再到除了log还有源码  
研究目标就是行为建模、故障诊断等等  

## Python

### PDF4FundingTools
为了方便项目申请、填报等工作，减少工作量，节省时间

**功能需求：** 
- 抽取特定页码，可以指定文件名、指定文件夹、指定输出文件名、指定输出文件夹、指定页码范围（如有些项目申请，需要论文首页做附件）
- 合并文件（有时候需要合并附件）
- 压缩PDF大小（附件有时候有大小限制）

**实现方案：** 
采用Python实现，基于Python的各种开源库，参考GoAgent的实现方式，在项目中内置Python运行环境，方便使用和移植  
https://automatetheboringstuff.com/chapter13/  
https://www.binpress.com/tutorial/manipulating-pdfs-with-python/167  
https://code.google.com/archive/p/pdfsizeopt/  

## Chrome Extension

### FreeExportSoopat
[Soopat](http://www2.soopat.com/Home/Index)的专利检索结果可以导出为excel文档，但是这个功能是收费的，所以就想开发一个插件，可以免费导出检索结果。并不是黑他们的后台，而是直接根据前端数据生成excel内容。大致流程就是依次获取每个检索结果页面的内容，然后再整理成excel内容。Soopat分为好几种检索结果展示方式，其中“列表式”比较合适，每页的内容比较多，需要翻页的次数比较少。但是，默认结果页面只展示了一些关键信息，还有很多内容必须进到每个专利的详情页才能看到。所以，现在就比较麻烦，需要打开每个页面去获取那些信息吗？这样就需要依次打开很多页面，速度会很慢，用户体验很不好。这样的话，是不是写成爬虫更合适？

### PatentExport
直接从国家知识产权局的[专利检索及分析系统](http://www.pss-system.gov.cn/sipopublicsearch/portal/uiIndex.shtml)上导出专利检索结果。这个系统的数据最全，还可以免费下载全文。

### GoogleScholarExport
导出Google Scholar的检索结果，目标是达到专业文献检索数据库的水平。