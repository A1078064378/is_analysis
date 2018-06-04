# 接口：morescore  [返回](../README.md)
用例： [学生查看实验多项得分](../yongli/学生查看实验多项得分.md)

- 功能：
    返回学生所选学期与课程与实验的该实验的具体多项得分。
    
- 权限：
    学生：只能查看自己的成绩，即接口参数student_id必须等于登录学生的student_id
    
- API请求地址： 
    接口基本地址/v1/api/moreScore/<student_id>

- 请求方式 ：
    GET

- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |student_id|学生的学号|
  |test_id|实验编号|
    
- 返回实例：

        {         
            "status": true,
            "info": null,    
            "student_id": "201510414120",  
            "test_id":1，
            "data": [
                {
                "title":"实验1:XXX"
                "result": 88, 
                "ecah_score":44,22,22
                "categories":"xxx"
                "Scoring criteria"："xxx"
                }，
            ] 
        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |student_id|学号| 
  |data|所有实验的成绩和评语|
  |test_id|实验编号|
  |result|本实验成绩，可以为空，为空表示没有批改，没有批改的实验不入平均成绩，为0分则要计入平均成绩，所以成绩为空和为0是不一样的。|
  |ecah_score|本实验多项得分成绩|
  |categories|本实验评分项|
  |Scoring criteria|本实验评分标准|
