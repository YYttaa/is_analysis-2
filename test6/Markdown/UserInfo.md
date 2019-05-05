# "查看用户信息"用例 | [返回][]

## 1.用例规约

<table>
    <tr>
        <td width="150"> <b>&nbsp;用例名称</b></td>
        <td colspan="2" width="700">&nbsp;查看用户信息</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;参与者</b></td>
        <td colspan="2" width="700">&nbsp;所有用户</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;前置条件</b></td>
        <td colspan="2" width="700">&nbsp;已在系统登录</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;后置条件</b></td>
        <td colspan="2" width="700">&nbsp;无</td>
    </tr>
    <tr>
        <td colspan="3" width="200"> <b>&nbsp;主事件流</b></td>
    </tr>
    <tr>
        <td colspan="2" width="180"> <b>&nbsp;参与者动作</b></td>
        <td width="410"> <b>&nbsp;系统行为</b></td>
    </tr>
    <tr>
        <td colspan="2" width="180">
            <span>&nbsp;1.用户选择查看用户信息；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;3.用户确认查看信息；</span>
        </td>
        <td width="480">
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;2.系统查询当前用户信息并返回至页面；</span>
            <br>
            <span>&nbsp;</span>
        </td>
    </tr>
    <tr>
        <td colspan="3" width="200"> <b>&nbsp;备选时间流</b></td>
    </tr>
    <tr>
        <td colspan="3" width="200">
            <span>&nbsp;2a.用户信息查询失败</span>
            <br>
            <span>&nbsp;&emsp;1.提示用户查询结果，返回第1步</span>
        </td>
    </tr>
    <tr>
        <td colspan="3" width="200"> <b>&nbsp;业务规则</b></td>
    </tr>
    <tr>
        <td colspan="3" width="200">
            <span>&nbsp;1.用户在进行登录后选才能进行查看当前用户的信息。</span>
            <br>
            <span>&nbsp;2.用户的隐秘信息应当使用*来进行保护。</span>
        </td>
    </tr>
</table>

<br>

## 2.业务流程(顺序图) | [源码](../puml/UserInfo.puml)
![img](../picture/UserInfoSe.png)

<br>

## 3.界面设计
* 界面参照:[https://tyh97.github.io/is_analysis_terminal_pages/userinfo.html](https://tyh97.github.io/is_analysis_terminal_pages/userinfo.html)
* API接口调用
    * 接口1:[userInfo](../interface/UserInfoInter.md)
    
    
<br>

## 4.算法描述
无

## 5.参照表
* [Students](../Markdown/DataBase.md#students学生表)
* [Teachers](../Markdown/DataBase.md#teachers教师表)
* [Manager](../Markdown/DataBase.md#manager管理员表)