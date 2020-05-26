# 接口getstudent  [返回](../README.md)



<ul>
    <li>权限：只能查看自己已选课程的学生列表，即接口参数lesson_id所对应lesson表中的lesson.teacher_id必须等于登录教师的teacher_id。</li>
    <li>功能：用于查看学生列表</li>
    <li>请求方法：POST</li>
    <li>
        请求实例：  
            
```
{
    "access_token": $access_token,
    "method": "POST",
    "lesson_id": 1
}
```
   </li>
    <li>
        请求参数：
        <table>
            <tr>
                <td>参数名称</td>
                <td>必填</td>
                <td>说明</td>
            </tr>
            <tr>
                <td>access_token</td>
                <td>是</td>
                <td>用于验证请求合法性的认证信息。</td>
            </tr>
            <tr>
                <td>method</td>
                <td>是</td>
                <td>固定为“POST”。</td>
            </tr>
            <tr>
                <td>lesson_id</td>
                <td>是</td>
                <td>课程的id，对应表lesson.lesson_id的值。</td>
            </tr>
        </table>
    </li>
    <li>
        返回实例：  
            
```
{
    "information": "查看学生列表成功",
    "status": true,
    "student_list": [
        {"student_id": "201710414315", "user_name":"啊啊啊", "github_name":"xxx"},
        {"student_id": "201710414316", "user_name":"哈哈哈", "github_name":"xxx"},
        {"student_id": "201710414317", "user_name":"嘻嘻嘻", "github_name":"xxx"},
    ],
    "code": 200
}
```
   </li>
    <li>
        返回参数说明：
        <table>
            <tr>
                <td>参数名称</td>
                <td>必填</td>
                <td>说明</td>
            </tr>
            <tr>
                <td>information</td>
                <td>是</td>
                <td>返回的说明信息。</td>
            </tr>
            <tr>
                <td>status</td>
                <td>是</td>
                <td>返回的结果，boolean类型，true表示正确的返回，false表示有错误。</td>
            </tr>
            <tr>
                <td>student_list</td>
                <td>否</td>
                <td>获取的学生列表。</td>
            </tr>
            <tr>
                <td>code</td>
                <td>是</td>
                <td>返回码。</td>
            </tr>
        </table>
    </li>
</ul>