# StuInfoManageSystem
大四「Web应用程序设计与开发」课程大作业
  
（一）  
我建立了stu_db数据库，其中包括三个数据表：  
StuInfo存储学生的个人信息（学号、姓名、性别、民族、生日、政治面貌、身份证号、手机、邮箱、qq）  
StuMajor存储学生的学籍信息（学历、学制、学院、专业、班级）  
StuScore存储学生的成绩信息（通信工程、数据结构、计算机网络三科的成绩）  
数据库中存储了学号从2016210001到2016210060共60个学生的信息  
  
  
（二）操作步骤  
输入链接 http://localhost/StuInfoManageSystem/main.php?page=1 进入主页面  
共分页成6页，每页展示10个学生的信息。  
  
1.增  
在主页面上点击“增加学生”，进入填写表单的界面  
填写完毕后，点击“提交”即可，再点击最下方的HOME按键可返回主页面。若填写错误，可点击“重置”。  
  
2.删  
点击主页面每个学生对应行的“删除”，即可删去该学生的全部信息。  
  
3.查  
分别点击主页面每个学生对应行的“个人信息”、“学籍信息”、“成绩信息”，即可进入相应页面查看该学生的对应信息。  
点击页面下方HOME返回主页面。  
  
4.改  
在查看信息页点击“编辑”按钮，可修改该学生的信息（注意只能改学生的信息，所以不能改学号）  
改好后，点击“保存”，即将数据更新至数据库  
（由于成绩信息一般只读不改，所以成绩信息页面没有设置编辑、保存按钮）  
点击页面下方HOME返回主页面。  
  
  
（三）分块解释  
main.php——生成主页面上的表格，用于链接到分页面
AddInfo.php——添加用户信息的页面
studentInfo.php——显示学生个人信息的页面
SaveStuInfo.php——保存更改后的学生个人信息，并更新至数据库
schoolMsg.php——保存更改后的学生学籍信息，并更新至数据库
studentGradeInfo.php——保存更改后的学生学籍信息，并更新至数据库
images——页面背景图片
css、js——这里主要参考了网络上的源码


（四）相比于课上的示例所做的后续工作
1.对显示数据进行了表格化
2.PHP 上的FORM上除了“Submit ”以外还添加了“Reset ”，用于重置
3.给所有分页面都添加了“HOME”用于返回主页面。
4.增加更多的HTML 元素使页面更便于使用
5.主页上显示的用户信息采用了分页算法 
