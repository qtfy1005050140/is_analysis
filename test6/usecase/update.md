# “修改用户信息”用例 [返回](../README.md)
## 1. 用例规约

|用例名称|修改用户信息|
|-------|:-------------|
|功能|修改用户的GitHub用户名称|
|参与者|学生，老师|
|前置条件|必须先登录，并且查看用户现有的GitHub用户名|
|后置条件| |
|主事件流| 1.用户填写GitHub用户名称 <br/> 2.用户提交修改信息 <br/>3.系统存储修改后的GitHub用户名称|
|备选事件流|1a. 如果用户输入的GitHub用户名称为空 <br/>&nbsp;&nbsp; 1.系统清空用户的GitHub用户名称|

## 2. 业务流程
无

## 3. 界面设计
- 界面参照: [界面](https://qtfy1005050140.github.io/is_analysis_pages/ui2/top.html)
- API接口调用
    - 接口1：[getUserInfo](../api/getUserInfo.md)
    - 接口2：[setUserInfo](../api/setUserInfo.md)
    

    
## 4. 参照表
- [table_user](../database/database.md)