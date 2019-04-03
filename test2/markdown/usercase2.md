# 取消预约预定表 | [返回](../README.md) | [下一张表](./usercase3.md)
<table>
    <tr>
        <td width="150"> <b>&nbsp;用例名称</b></td>
        <td colspan="2" width="600">&nbsp;取消预定</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;参与者</b></td>
        <td colspan="2" width="600">&nbsp;读者</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;前置条件</b></td>
        <td colspan="2" width="600">&nbsp;读者预定图书</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;后置条件</b></td>
        <td colspan="2" width="600">&nbsp;无</td>
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
            <span>&nbsp;5.选择需要被取消预定的图书；</span>
            <br>
            <span>&nbsp;6.确认取消图书；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;8.确认取消成功；</span>
        </td>
        <td width="410">
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;2.系统查询登录是被允许；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;4.系统显示已经预定的图书；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;7.显示取消预定成功；</span>
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
            <span>&nbsp;4a.系统未查询到预定图书</span>
            <br>
            <span>&nbsp;&emsp;1.提示读者未约定图书，转第3步</span>
            <br>
            <span>&nbsp;7a.取消预定失败</span>
            <br>
            <span>&nbsp;&emsp;1.提示取消预定错误信息，转第5步</span>
        </td>
    </tr>
    <tr>
        <td colspan="3" width="200"> <b>&nbsp;业务规则</b></td>
    </tr>
    <tr>
        <td colspan="3" width="200">
            <span>&nbsp;1.用户登录成功后可以查询自己所预定的图书，并选择取消</span>
            <br>
            <span>&nbsp;2.读者所预定的图书为空时，返回主界面</span>
        </td>
    </tr>
</table>