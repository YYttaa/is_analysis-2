# 查询书目规约表 | [返回](../README.md) | [下一张表](./usercase6.md)
<table>
    <tr>
        <td width="150"> <b>&nbsp;用例名称</b></td>
        <td colspan="2" width="600">&nbsp;查询书目</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;参与者</b></td>
        <td colspan="2" width="600">&nbsp;读者</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;前置条件</b></td>
        <td colspan="2" width="600">&nbsp;图书存在</td>
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
            <span>&nbsp;1.读者选择查询方式；</span>
            <br>
            <span>&nbsp;2.输入查询内容</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;4.读者查看书目信息，用例结束；</span>
        </td>
        <td width="410">
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;3.系统返回书目信息；</span>
            <br>
            <span>&nbsp;</span>
        </td>
    </tr>
    <tr>
        <td colspan="3" width="200"> <b>&nbsp;备选时间流</b></td>
    </tr>
    <tr>
        <td colspan="3" width="200">
            <span>&nbsp;2a.没有查询到指定书目</span>
            <br>
            <span>&nbsp;&emsp;1.提示查询信息，返回第1步</span>
        </td>
    </tr>
    <tr>
        <td colspan="3" width="200"> <b>&nbsp;业务规则</b></td>
    </tr>
    <tr>
        <td colspan="3" width="200">
            <span>&nbsp;1.只有图书存在时才能被查询，否则返回空白信息</span>
            <br>
            <span>&nbsp;2.读者可以通过多种方式进行查询，例如模糊查询，精准查询</span>
        </td>
    </tr>
</table>