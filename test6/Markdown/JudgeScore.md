# "评定成绩"用例 | [返回](../README.md#6)

## 1.用例规约

<table>
    <tr>
        <td width="150"> <b>&nbsp;用例名称</b></td>
        <td colspan="2" width="700">&nbsp;评定成绩</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;参与者</b></td>
        <td colspan="2" width="700">&nbsp;教师</td>
    </tr>
    <tr>
        <td width="150"> <b>&nbsp;前置条件</b></td>
        <td colspan="2" width="700">&nbsp;学生选择课程</td>
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
            <span>&nbsp;1.教师发起评分请求；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;3.教师选择需要评分的课程；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;5.教师选择需要进行评分的学生；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;7.教师对学生实验进行评分；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;9.教师确认评分，用例结束；</span>
        </td>
        <td width="480">
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;2.系统返回本学期教师所教授的课程；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;4.系统返回选择本课程的学生目录；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;6.系统返回所选择学生的实验信息；</span>
            <br>
            <span>&nbsp;</span>
            <br>
            <span>&nbsp;8.系统存储学生的评分信息，并实时将学生的分数合计到该课程分数；</span>
            <br>
            <span>&nbsp;</span>
        </td>
    </tr>
    <tr>
        <td colspan="3" width="200"> <b>&nbsp;备选时间流</b></td>
    </tr>
    <tr>
        <td colspan="3" width="200">
            <span>&nbsp;8a.评分失败</span>
            <br>
            <span>&nbsp;&emsp;1.提示教师评分失败，返回第7步</span>
        </td>
    </tr>
    <tr>
        <td colspan="3" width="200"> <b>&nbsp;业务规则</b></td>
    </tr>
    <tr>
        <td colspan="3" width="200">
            <span>&nbsp;1.教师需要根据实验所给的地址自行点进学生实验界面。</span>
            <br>
            <span>&nbsp;2.教师需要根据所给的评分细则进行评分。</span>
        </td>
    </tr>
</table>

<br>

## 2.业务流程(顺序图) | [源码](../puml/LoginInfo.puml)
![img](../picture/LoginInfoSe.png)