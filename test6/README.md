# 基于GitHub的实验管理平台的分析与设计

### 成都大学信息科学与工程学院

|学号|班级|姓名|照片|
|:-------:|:-------------: | :----------:|:---:|
|201510414220|软件(本)15-2   |巫恒强 |<img src="images/xiaoqiang.jpg" width="20%" height="20%" />|

## 1. 概述(三单改三多)
- 基于GitHub的实验管理平台的作用是在线管理实验成绩的Web应用系统。学生和老师的实验内容均存放在GitHUB
页面上。
- 学生的功能主要有：一是设置自己的GitHub用户名，二是查询自己的实验成绩。学生的GitHub用户名是公开的，但成绩不公开。
- 老师的功能主要有：一是批改每个学生的成绩，二是查看每个学生的成绩。
- 老师和学生都能通过本系统的链接方便地跳转到学生的每个GitHUB实验目录，以便批改实验或者查看实验情况。
- 实验成绩按数字分数计算，每项实验的满分为100分，最低为0分。
- 系统自动计算每个学生的所有实验的平均分。
- 一个老师可以上多门课，每个老师只能维护老师自己的课程及成绩。
- 一人同学可以上多门课，每个同学只能查询同学自己的课程的实验成绩。
- 必须考虑选课了，老师和同学都可以选多门课程，但必须是老师先选，学生后选。
- 原实验为单评分项实验，要求改为多评分项实验，即每个实验的实验成绩细分为多个评分项，每个评分项对应各自的评分标准。 老师在批改实验的时候，对每个评分项进行评分并输入对应的文字评价，系统自动计算出所有评分项的成绩之和为该实验的总成绩。
- 考虑到有多个学期，每个学期都有不同的实验。
- 系统设计在界面上和操作上应该方便老师查询和评阅学生的实验成绩，应该方便学生查询实验成绩。
## 2. 系统总体结构
![](images_s/系统总体结构.png)

界面设计参见：https://wuhengqiang100.github.io/is_analysis/test6/ui/index.html
    
## 3. 用例图设计 [源码](src/用例图.puml)
![](images_s/用例图.png)

## 4. 类图设计 [源码](src/类图.puml)
![](images_s/类图.png)

## 5. 数据库设计
- ### [参见数据库设计](数据库设计/数据库设计.md)

## 6. 用例及界面详细设计
- ### [“评定成绩”用例](./用例/评定成绩.md),[界面](https://wuhengqiang100.github.io/is_analysis/test6/ui/评定成绩.html)
- ### [“查看学生列表”用例](./用例/学生列表.md),[界面](https://wuhengqiang100.github.io/is_analysis/test6/ui/index.html)
- ### [“选择学期”用例](./用例/查询学期.md),[界面](https://wuhengqiang100.github.io/is_analysis/test6/ui/查看成绩.html)
- ### [“选择课程”用例](./用例/查询课程.md),[界面](https://wuhengqiang100.github.io/is_analysis/test6/ui/查看成绩.html)
- ### [“查看成绩”用例](./用例/查看成绩.md),[界面](https://wuhengqiang100.github.io/is_analysis/test6/ui/查看成绩.html)
- ### [“修改密码”用例](./用例/修改密码.md),[界面](https://wuhengqiang100.github.io/is_analysis/test6/ui/修改密码.html)
- ### [“修改用户信息”用例](./用例/修改用户信息.md),[界面](https://wuhengqiang100.github.io/is_analysis/test6/ui/个人信息.html)
- ### [“查看用户信息”用例](./用例/查看用户信息.md),[界面](https://wuhengqiang100.github.io/is_analysis/test6/ui/个人信息.html)
- ### [“登出”用例](./用例/登出.md),[界面](https://wuhengqiang100.github.io/is_analysis/test6/ui/安全退出.html)
- ### [“登录”用例](./用例/登录.md),[界面](https://wuhengqiang100.github.io/is_analysis/test6/ui/login.html)
    