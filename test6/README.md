# 实验6：基于GitHub的实验管理平台的分析与设计
|学号|班级|姓名|照片|
|:-------:|:-------------: | :----------:|:---:|
|201510414120|软件(本)15-1|魏金冰|![flow1](timg.jpg)|

## 1. 概述
- 基于GitHub的实验管理平台的作用是在线管理实验成绩的Web应用系统。学生和老师的实验内容均存放在GitHUB
页面上。
- 学生的功能主要有：设置自己的GitHub用户名和密码，之后可以进行登录和修改，登录后可看到自己的实验成绩，可以通过选择不同学期，不同课程查看其他学期和课程的成绩。点击一项实验成绩时，可以看到各个评分项的具体得分。
- 老师的功能主要有：以老师身份登录后，可以看到学生成绩列表和批改状态，可以对其进行评分和修改，可以通过选择不同学期，不同课程查看和修稿其他学期和课程的成绩。进入评分时为多项评分，并需要给出评语。
- 老师和学生都能通过本系统的链接方便地跳转到学生的每个GitHUB实验目录，以便批改实验或者查看实验情况。
- 实验成绩按数字分数计算，每项实验的满分为100分，最低为0分。
- 系统自动计算每个学生的所有实验的平均分。
    
## 2. 系统总体结构
![](系统总体结构.png)

界面设计参见：https://a1078064378.github.io/is_analysis/test6/ui/index.html
    
## 3. 用例图设计 [源码](src/用例图.puml)
![](用例图.png)

## 4. 类图设计 [源码](src/leitu1.puml)
![](leitu1.png)

## 5. 数据库设计
- ### [参见数据库设计](./数据库设计.md)

## 6. 用例及界面详细设计
- ### [“登录”用例](./yongli/登录.md),[界面](https://A1078064378.github.io/is_analysis/test6/ui/index.html)
- ### [“登出”用例](./yongli/登出.md),[界面](https://A1078064378.github.io/is_analysis/test6/ui/student.html)
- ### [“选择学期”用例](./yongli/选择学期.md),[界面](https://A1078064378.github.io/is_analysis/test6/ui/student.html)
- ### [“选择课程”用例](./yongli/选择课程.md),[界面](https://A1078064378.github.io/is_analysis/test6/ui/student.html)
- ### [“修改密码”用例](./yongli/修改密码.md),[界面](https://A1078064378.github.io/is_analysis/test6/ui/information.html)
- ### [“学生查看科目成绩”用例](./yongli/学生查看科目成绩.md),[界面](https://A1078064378.github.io/is_analysis/test6/ui/student.html)
- ### [“学生查看实验多项得分”用例](./yongli/学生查看实验多项得分.md),[界面](https://A1078064378.github.io/is_analysis/test6/ui/duopingfen.html)
- ### [“学生成绩列表”用例](./yongli/学生成绩列表.md),[界面](https://A1078064378.github.io/is_analysis/test6/ui/teacher.html)
- ### [“评分”用例](./yongli/评分.md),[界面](https://A1078064378.github.io/is_analysis/test6/ui/piyue.html)

