# 接口：studentlist  [返回](../README.md)
用例： [学生成绩列表](../yongli/学生成绩列表.md)

- 权限：
    仅老师可查看

- 功能：
    返回该学期该科目该实验下所有学生的成绩信息。

- API请求地址：
   接口基本地址/v1/api/studentList

- 请求方式 ：
    GET

- 请求参数说明:
    无

- 返回实例：

        {
            "status": true,
            "info": null,
            "total": 121,
            "data": [
                {
                 "STUDENT_ID": "001",
                 "NAME": "张三",
                 "GITHUB_USERNAME": "10086",
                 "RESULT": "77",
                 "state":"已批阅",
                   "UPDATE_DATE": "2018-04-02 13:48:01"},
                {
                ...其他学生
                }
            ]
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |total|返回学生人数|
  |data|所有学生的数组|
  |RESULT|最终成绩|
  |GITHUB_USERNAME|GITHUB 用户名|
  |STUDENT_ID|学号|
  |NAME|真实姓名|
  |STATE|批改状态|
  |UPDATE_DATE|GitHUB用户名修改日期|
