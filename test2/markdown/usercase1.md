# 反馈信息规约表 | [返回](../README.md)
<table>
    <tr>
        <td width="150"> <b>&nbsp;用例名称</b></td>
        <td colspan="2" width="500">&nbsp;反馈信息</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;参与者</b></td>
        <td colspan="2" width="500">&nbsp;读者</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;前置条件</b></td>
        <td colspan="2" width="500">&nbsp;无</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;后置条件</b></td>
        <td colspan="2" width="500">&nbsp;无</td>
    </tr>
    <tr>
        <td colspan="3" width="150"> <b>&nbsp;主事件流</b></td>
    </tr>
    <tr>
        <td colspan="2" width="200"> <b>&nbsp;参与者动作</b></td>
        <td width="400"> <b>&nbsp;系统行为</b></td>
    </tr>
    <tr>
        <td colspan="2" width="200">
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;2.读者选择反馈的信息种类</span>
            <br>
            <span>&nbsp;3.填写反馈信息</span>
            <br>
            <span>&nbsp;4.读者确认填写完毕，提交反馈信息</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;6.读者确认反馈成功，用例结束</span>
            <br>
        </td>
        <td width="400">
            <span>&nbsp;1.系统显示需要反馈的信息的种类</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;5.将反馈信息保存并发给管理员</span>
            <br>
            <span>&nbsp;</span>
        </td>
    </tr>
    <tr>
        <td colspan="3" width="150"> <b>&nbsp;备选时间流</b></td>
    </tr>
    <tr>
        <td colspan="3" width="150">
            <span>&nbsp;3a.读者取消填写</span>
            <br>
            <span>&nbsp;&emsp;1.系统清空所有输入，回到初始界面</span>
            <br>
            <span>&nbsp;4a.读者选择重填</span>
            <br>
            <span>&nbsp;&emsp;1.系统清空所有输入，转第2步</span>
            <br>
            <span>&nbsp;6a.读者反馈失败</span>
            <br>
            <span>&nbsp;&emsp;1.输出错误提示，转第1步</span>
        </td>
    </tr>
    <tr>
        <td colspan="3" width="150"> <b>&nbsp;业务规则</b></td>
    </tr>
    <tr>
        <td colspan="3" width="150">
            <span>&nbsp;1.用户可以反馈多种信息，并可以看到是否反馈成功。</span>
            <br>
            <span>&nbsp;2.管理员收到读者反馈的信息后进行处理。</span>
        </td>
    </tr>
</table>