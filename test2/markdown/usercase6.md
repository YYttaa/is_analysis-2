# 增加图书信息规约表 | [返回](../README.md) | [下一张表](./usercase7.md)
<table>
    <tr>
        <td width="150"> <b>&nbsp;用例名称</b></td>
        <td colspan="2" width="600">&nbsp;增加图书信息</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;参与者</b></td>
        <td colspan="2" width="600">&nbsp;图书管理员</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;前置条件</b></td>
        <td colspan="2" width="600">&nbsp;图书未存在</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;后置条件</b></td>
        <td colspan="2" width="600">&nbsp;将图书信息加入到可借阅表中</td>
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
            <span>&nbsp;3.管理员选择增加图书功能；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;5.管理员填入图书的各项信息并提交；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;7.管理员确认增加结果，用例结束；</span>
        </td>
        <td width="410">
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;2.系统查询登录是否被允许；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;4.系统列出添加图书的各项信息；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;6.系统存储图书信息并反馈存储结果；</span>
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
            <span>&nbsp;5a.管理员重填信息</span>
            <br>
            <span>&nbsp;&emsp;1.清空填入信息，返回第5步</span>
            <br>
            <span>&nbsp;5b.管理员取消填入信息</span>
            <br>
            <span>&nbsp;&emsp;1.清空填入信息，返回第3步</span>
            <br>
            <span>&nbsp;6a.系统存入信息出错</span>
            <br>
            <span>&nbsp;&emsp;1.显示错误信息，返回第3步</span>
        </td>
    </tr>
    <tr>
        <td colspan="3" width="200"> <b>&nbsp;业务规则</b></td>
    </tr>
    <tr>
        <td colspan="3" width="200">
            <span>&nbsp;1.只有图书未存在时才能被增加，否则返回错误信息</span>
            <br>
            <span>&nbsp;2.读者在填写图书信息时应该选择图书的分类，并验证图书的ISBN码</span>
        </td>
    </tr>
</table>