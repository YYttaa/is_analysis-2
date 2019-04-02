# 维护书目规约表 | [返回](../README.md)
<table >
    <tr>
        <td width="150"> <b>&nbsp;用例名称</b></td>
        <td colspan="2" width="700">&nbsp;维护书目</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;参与者</b></td>
        <td colspan="2" width="700">&nbsp;图书管理员</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;前置条件</b></td>
        <td colspan="2" width="700">&nbsp;管理员登录</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;后置条件</b></td>
        <td colspan="2" width="700">&nbsp;将修改后的图书信息更新到系统</td>
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
            <span>&nbsp;1.管理员登录；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;3.管理员进入维护图书功能；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;5.管理员选择对图书的具体维护功能；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;7.管理员对图书进行操作，并提交；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;9.管理员确认更新，用例结束；</span>
        </td>
        <td width="500">
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;2.系统查询登录是否被允许；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;4.系统列出各项对图书的维护功能；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;6.系统根据所选择的功能显示功能界面；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;8.系统将更改的书目信息进行更新，并反馈更新结果；</span>
            <br>
            <span>&nbsp;</span>
        </td>
    </tr>
    <tr>
        <td colspan="3" width="200"> <b>&nbsp;备选时间流</b></td>
    </tr>
    <tr>
        <td colspan="3" width="200">
            <span>&nbsp;2a.管理员密码错误</span>
            <br>
            <span>&nbsp;&emsp;1.提示查询信息，返回第1步</span>
            <br>
            <span>&nbsp;5a.管理员退出图书维护功能</span>
            <br>
            <span>&nbsp;&emsp;1.清除界面，返回第3步</span>
            <br>
            <span>&nbsp;7a.管理员重新选择图书维护功能</span>
            <br>
            <span>&nbsp;&emsp;1.清空选择信息，返回第5步</span>
            <br>
            <span>&nbsp;7b.管理员取消填入信息</span>
            <br>
            <span>&nbsp;&emsp;1.清空填入信息，返回第7步</span>
            <br>
            <span>&nbsp;8a.系统更新书目信息出错</span>
            <br>
            <span>&nbsp;&emsp;1.显示错误信息，返回第5步</span>
        </td>
    </tr>
    <tr>
        <td colspan="3" width="200"> <b>&nbsp;业务规则</b></td>
    </tr>
    <tr>
        <td colspan="3" width="200">
            <span>&nbsp;1.管理员只有在登录的情况下才能进行修改，否则返回登录界面</span>
            <br>
            <span>&nbsp;2.可以提供管理员的忘记密码功能</span>
            <br>
            <span>&nbsp;3.系统应该提供多种对书目进行维护的操作，例如更新，增加，删除等操作</span>
            <br>
            <span>&nbsp;4.系统应该验证管理员所输入的数据的合法性，并及时提示管理员</span>
        </td>
    </tr>
</table>