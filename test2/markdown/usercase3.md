# 预定图书规约表 | [返回](../README.md) | [下一张表](./usercase4.md)
<table >
    <tr>
        <td width="150"> <b>&nbsp;用例名称</b></td>
        <td colspan="2" width="600">&nbsp;预定图书</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;参与者</b></td>
        <td colspan="2" width="600">&nbsp;读者</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;前置条件</b></td>
        <td colspan="2" width="600">&nbsp;读者已注册</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;后置条件</b></td>
        <td colspan="2" width="600">&nbsp;系统对读者借阅信息进行更改</td>
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
            <span>&nbsp;1.读者登录系统；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;3.读者查询图书；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;5.选择需要预定的图书；</span>
            <br>
            <span>&nbsp;6.确认预定图书；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;9.读者确认预定成功，用例结束；</span>
        </td>
        <td width="410">
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;2.系统查询登录是被允许；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;4.系统显示搜寻的图书；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;7.系统更改读者借阅情况；</span>
            <br>
            <span>&nbsp;8.返回预定成功消息；</span>
            <br>
            <span>&nbsp;</span>
        </td>
    </tr>
    <tr>
        <td colspan="3" width="200"> <b>&nbsp;备选时间流</b></td>
    </tr>
    <tr>
        <td colspan="3" width="200">
            <span>&nbsp;2a.读者密码错误</span>
            <br>
            <span>&nbsp;&emsp;1.系统返回登录界面，转第1步</span>
            <br>
            <span>&nbsp;2b.读者未注册</span>
            <br>
            <span>&nbsp;&emsp;1.系统返回登录界面，转第1步</span>
            <br>
            <span>&nbsp;4a.系统未查询到图书</span>
            <br>
            <span>&nbsp;&emsp;1.提示读者未搜寻到图书，转第3步</span>
            <br>
            <span>&nbsp;6a.读者重新选择预定图书</span>
            <br>
            <span>&nbsp;&emsp;1.清空搜寻信息，转第3步</span>
            <br>
            <span>&nbsp;7a.修改读者信息失败</span>
            <br>
            <span>&nbsp;&emsp;1.提示读者错误信息，转第3步</span>
        </td>
    </tr>
    <tr>
        <td colspan="3" width="200"> <b>&nbsp;业务规则</b></td>
    </tr>
    <tr>
        <td colspan="3" width="200">
            <span>&nbsp;1.用户登录成功后可以查询图书，并选择预定</span>
            <br>
            <span>&nbsp;2.一位读者同时能够在借图书本数为10本</span>
            <br>
            <span>&nbsp;3.一位读者一次性可以借阅多本图书，但是不能超过借阅上限</span>
        </td>
    </tr>
</table>