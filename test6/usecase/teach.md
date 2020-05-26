# “老师选课”用例 [返回](../README.md)
## 1. 用例规约

<table>
    <caption>“老师选课”用例规约</caption>
    <tr>
        <td>用例名称</td>
        <td>老师选课</td>
    </tr>
    <tr>
        <td>参与者</td>
        <td>老师</td>
    </tr>
    <tr>
        <td>前置条件</td>
        <td>老师已登录</td>
    </tr>
    <tr>
        <td>后置条件</td>
        <td>系统跳转至实验管理平台首页</td>
    </tr>
    <tr>
        <td colspan="2">主事件流</td>
                <td>
                    1. 老师点击选课按钮；<br>
                     2. 系统验证老师登录状态是否有效；<br>
                     3. 系统检索能够被老师选择的课程；<br>
                     4. 系统返回课程列表；<br>
                     5. 系统跳转至选课页面；<br>
                     6. 老师选择课程；<br>
                     7. 老师点击提交按钮；
                     8. 系统存储老师选择的课程；<br>
                     9. 系统提示选课成功。      
                </td>
    </tr>
    <tr>
        <td colspan="2">备选事件流</td>
                <td colspan="2">
                    2a. 系统验证老师登录状态已失效<br>
                        &nbsp&nbsp&nbsp&nbsp&nbsp&nbsp
                        1. 系统提示验证老师登录状态失败，转第1步；<br>
                    4a. 系统未能检索到能够被学生选择的课程<br>
                        &nbsp&nbsp&nbsp&nbsp&nbsp&nbsp
                        1. 系统提示无可选课程，转第1步；<br>。
                </td>
    </tr>
</table>


## 2. 业务流程（顺序图） 

无
    
## 3. 界面设计
- 界面参照: [界面](https://qtfy1005050140.github.io/is_analysis_pages/ui2/teach.html)

- API接口调用

    - 接口1：[chooseLesson](../api/chooseLesson.md)
        
        老师选课
        


    
## 4. 参照表
- [table_lesson](../database/database.md)
- [table_teacher](../database/database.md)
- [table_test](../database/database.md)