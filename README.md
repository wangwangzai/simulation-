此疫情仿真程序采用Java语言所写，图形界面由Java swing包中的各种UI组件构成，地图为一个方形区域，里面随机散落着5000个人员，初始时有100个感染者，每过一秒更新下。
人员的状态分为5种，分别为正常、潜伏、感染、在医院隔离，死亡。  

主要变量为：人员流动意向，戴口罩，自我隔离。  

人员流动意向由一个方差为1，均值自我修改的正态分布控制，随机出来的数大于0则有意向流动，小于0则无。当均值为0.99时，大部分人会流动，-0.99时大部分人不会进行流通。  

戴口罩这个变量由感染的距离控制，若带上口罩，则不易被感染。  

自我隔离时，感染的人员不会移动也不会感染他人。  


通过修改变量，对比结果：  

如果控制不了疫情，对比感染人数超过80%所需的时间。  

如果成功控制疫情，对比剩余健康者的人数

1  人员倾向于流动， 发病者不隔离 ， 不带口罩  

![image](https://user-images.githubusercontent.com/49340916/109908054-8e7be400-7cde-11eb-91a7-f29fefd13e7d.png)  

2，一般人员不流动，发病者不隔离，不带口罩  

![image](https://user-images.githubusercontent.com/49340916/109908139-ae130c80-7cde-11eb-93c9-f9bdef4ac299.png)  
3，人员不倾向于流动，发病者隔离，不带口罩  
![image](https://user-images.githubusercontent.com/49340916/109908325-0b0ec280-7cdf-11eb-94e8-9194c6b78a0f.png)  
4 人员不倾向于流动，发病者隔离，带口罩  
![image](https://user-images.githubusercontent.com/49340916/109908346-1235d080-7cdf-11eb-8760-a0aa52d528fb.png)  
5，全体人员倾向于流动，自我隔离 ，带口罩  
![image](https://user-images.githubusercontent.com/49340916/109908372-1eba2900-7cdf-11eb-8cca-af928e897ab5.png)  
6，全城隔离  
![image](https://user-images.githubusercontent.com/49340916/109908394-2a0d5480-7cdf-11eb-9ece-58c4a7d3cdb6.png)





