# DAOrayaki 内容管理
## 总览
### 分支结构
DAOrayaki共有两个分支：

** 主分支（main） **
存储已发布的正式内容

** 工作分支（develop） **
存储正在编写和审核的内容，审核通过后的文章将会被合并到主分支中。

### 目录结构
按照日期划分，如2021年第一季度中，2021年7月21日的任务将会被放到以下文件夹下：
```
content/2021/2021-Q1/2021-07-21
```

文件命名用日期 + <项目名称/文章名称>方式命名,非法字符如 ：用 _ 代替，如

```
2021-07-21-Quadratic voting_ How mechanism design can radicalize democracy
```

## 工作流程
### 任务发布
任务发布者需要发起"Weekly Task" 或者 "Special Task"任务，并将任务Assign给相应的负责人，内容格式如下：

```
project：

<name> : 
<project 1> : <project url>
<project 2> : <project url>
...
```

例如：

```
project:

unes： 
BitDAO：https://www.bitdao.io
DAOhaus: https://daohaus.club
ECONOMIC SPACE AGENCY：https://economicspace.agency

trans:

筱威:
Data Catalog 3.0: Modern Metadata for the Modern Data Stack （dewei 120u）
https://towardsdatascience.com/data-catalog-3-0-modern-metadata-for-the-modern-data-stack-ec621f593dcf
```

命名方式用<time> + Tasks来命名，如：
  
```
  2021-07-21 Tasks
```

### 贡献内容
贡献者需要将所完成文档内容上传到develop分支中相应目录下，并发起"Task Verification"，并将任务Assign给需要负责审核的人,格式如下：

```
投票地址：<微信/DISCORD/SNAPSHOT>

研究种类：<关键词>

原文作者: <原作者>

贡献者： <贡献者>

原文: <原文内容>
  
原文链接：<原文链接>
```
  
如：
  
```
  
投票地址：<微信/DISCORD/SNAPSHOT>

研究种类：DAO, Social networks, Sybil defenses, Survey

原文作者: Aziz Mohaisen, Joongheon Kim

贡献者： Natalie, DAOctor @DAOrayaki

原文: The Sybil Attacks and Defenses: A Survey
  
原文链接：<原文链接>
  
```
  
文档的命名使用 Will <文档访问地址> pass ?来命名，如：
  
 ```
  Will https://github.com/DAOrayaki/CONTENT/blob/main/2021/2021-Q3/2021-07-21/2021-07-21-%E6%B5%8B%E8%AF%95%E6%96%87%E6%A1%A3.txt pass?
 ```
