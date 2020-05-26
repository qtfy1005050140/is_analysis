# 登录用例 [返回](../README.md)
## 1.用例规约

<table>
    <caption>“登录”用例规约</caption>
    <tr>
        <td>用例名称</td>
        <td>登录</td>
    </tr>
    <tr>
        <td>参与者</td>
        <td>访客</td>
    </tr>
    <tr>
        <td>前置条件</td>
        <td>访客进入实验管理平台首页</td>
    </tr>
    <tr>
        <td>后置条件</td>
        <td>系统跳转至用户个人主页</td>
    </tr>
    <tr>
        <td colspan="2">主事件流</td>
                <td>
                    1. 访客进入登录界面；<br>
                    2. 访客选择用户类型；<br>
                    3. 访客输入用户名和密码；<br>
                    4. 系统判断用户名、密码、用户类型正确；<br>
                    5. 系统在客户端以cookie形式存储登录用户信息；<br>
                    6. 系统提示访客登录成功
                </td>
    </tr>
    <tr>
        <td colspan="2">备选事件流</td>
        <td> 2a. 访客未选择用户类型<br>
                            &nbsp&nbsp&nbsp&nbsp&nbsp&nbsp
                            1. 系统提示选择用户类型，转第2步；<br>
                        3a. 访客未输入用户名<br>
                            &nbsp&nbsp&nbsp&nbsp&nbsp&nbsp
                            1. 系统提示输入用户名，转第3步；<br></td>
    </tr>

</table>

## 2.业务流程
无

## 3.界面设计
- 界面参照:[界面](https://qtfy1005050140.github.io/is_analysis_pages/ui2/login.html)
- API接口调用:[login](../api/login.md)

## 4.参照表
- [table_user](../database/database.md)