# 題目:大學生網上訂餐系統
![目錄](https://github.com/curryluku/SE_Final-Paper/assets/91310381/467fa1ba-a1a8-41ba-8dd8-e0a41a78c052)
# 1.背景介绍
随着网络技术的飞速发展,人们的生活也越来越追求方便化。经过观察,发现整个大学城的学生对平常订餐需求很大, 但他们订餐的方式都是比较原始的电话订餐。而各个餐饮店也是各自为战,自己接电话,记录订单需求,自己配送。这样做效率很低、利润薄,而且信息不流畅。所以我决定为大学生提供一个平台 --- 网上订餐系统。在网上给申请的商家一个虚拟店面,可以在上面挂上该商家的名称,饭菜的图片和价格等信息,让订餐者可以方便地订餐,还可以对商家的 餐饮进行评价,由系统生成评价档案以供其他人参考等,而商家后期只负责做饭 菜并安排人配送。此外,需要定期对商家进行卫生安全监察,生成商家监察档案, 并以此为依据来决定商家的去留等。
# 2.需求分析
大学生网上订餐系统主要有以下几方面需求:

订餐者
订餐者首先需要注册一个账号用于系统登录,登录后可以查看店铺信息,并选中某一店铺后进入其餐饮信息界面,最终选中所需餐饮,下订单。当然用餐后还可以对此餐饮进行评价。

商家
商家首先需要申请一个网上店铺,当申请通过后,登录到系统中,可以核实订单并安排配送,然后对本店的餐饮信息进行更新。

订单管理员
当订餐者下订单后,订单管理员需及时生成订单,如果订餐者对订单有所更改时,订单管理员也要及时对数据进行更新。

店铺管理员
当商家申请通过时,店铺管理员需要及时录入店铺信息,并为其设立店面、建立客户评价档案、商家监察档案。当商家增加、修改、删除其餐饮信息时,店铺管理员需及时对数据进行更新,以便其他人订餐。如果订餐者对某餐饮店的某餐饮进行评价后,店铺管理员需及时更新评价档案。

系统管理员
系统管理员主要完成对商家和订餐者信息的管理,以及系统的维护。

# 3.系统用例模型

大学生网上订餐系统的参与者有:

![1](https://github.com/curryluku/SE_Final-Paper/assets/91310381/797f5135-ae74-4ce1-9901-c6aceee637d2)

## 3.1 订餐者用例图

订餐者可以登录系统,登录后可以订餐,订餐过程包括选择店铺、选择餐饮、下订单以及到餐付款,用餐后还可以对餐饮进行评价。
![2](https://github.com/curryluku/SE_Final-Paper/assets/91310381/40bad2ff-06f0-4971-90de-8d0bd295b223)

## 3.2 商家用例图

商家可以登录系统,登录后需要对订餐者的订单进行核实并安排配送,然后更新店铺有关餐饮信息(增加、删除、修改)。
![3](https://github.com/curryluku/SE_Final-Paper/assets/91310381/f1d1d121-baef-42ff-8272-cff486ad47c6)

## 3.3 店铺管理员用例图

店铺管理员可以更新店铺信息(包括录入新申请通过的商家、修改、删除和 查询店铺信息),还要为每一个店铺建立客户评价档案盒商家监察档案。
![4](https://github.com/curryluku/SE_Final-Paper/assets/91310381/d9e0689a-e140-43ad-b3e9-c60c0098b20b)

## 3.4 订单管理员用例图

订单管理员当订餐者下订单后要立即生成新订单, 如果订单有所改动需及时更新(查询、修改、删除)。
![5](https://github.com/curryluku/SE_Final-Paper/assets/91310381/247965bc-7f76-4eb3-947e-b0a3f02f626b)

## 3.5 系统管理员用例图

系统管理员可以登录系统,对商家和订餐者的信息进行管理(增加、删除、 修改、查询),还有系统的维护。
![6](https://github.com/curryluku/SE_Final-Paper/assets/91310381/0f1f6e22-8168-4161-851c-caa4d67c7225)

# 4.系统静态模型
由需求分析中知,我们可以依据主要六个类对象:订餐者、订单管理员、商家、店铺管理员、系统管理员、订单、店铺和餐饮创建完整的类图。
![7](https://github.com/curryluku/SE_Final-Paper/assets/91310381/356cbcac-1a46-4769-a948-89c3a94b3713)

## 5.1.1 订餐者订餐
(1)订餐者注册一个系统登录账号:

(2)在登录界面输入相应的用户名和密码进行身份验证:

(3)系统验证后将验证结果返回给用户:

(4)系统展示有关店铺信息:

(5)订餐者选择店铺:

(6)系统展示该店铺的有关餐饮信息:

(7)订餐者浏览信息并选择所需餐饮:

(8)订餐者下订单:

(9)下订单成功后,系统更新餐饮信息:

(10)退出系统:

(11)用餐后对餐饮进行评价。

![8](https://github.com/curryluku/SE_Final-Paper/assets/91310381/6e19857c-833c-4e5a-9347-6924365df518)

根据订餐者订餐的时序图可以创建如下协作图:

![9](https://github.com/curryluku/SE_Final-Paper/assets/91310381/85a04af8-554c-4e51-8b77-720c72a08492)

## 5.1.2 商家管理店铺

(1)商家申请一个网上虚拟店铺:

(2)申请成功后,在登录界面输入自己的用户名和密码进行身份验证:

(3)系统进行验证并将验证结果返回给商家:

(4)商家处理订单:

(5)更新店铺相关餐饮信息:

(6)提交更新数据:

(7)系统将提交的结果显示给商家:

(8)提交成功,退出系统。

![10](https://github.com/curryluku/SE_Final-Paper/assets/91310381/b7254240-b3e1-4569-8304-0499331d7947)

根据商家管理店铺的时序图可以创建如下协作图:

![11](https://github.com/curryluku/SE_Final-Paper/assets/91310381/c99fd213-ebbe-4e82-bfb6-d518c31f2982)

## 5.1.3 店铺管理员管理店铺信息

(1)店铺管理员登录系统进入管理界面:

(2)对店铺的信息进行更新:

(3)提交更新数据:

(4)系统将提交结果显示给店铺管理员:

(5)提交成功,退出系统。

![12](https://github.com/curryluku/SE_Final-Paper/assets/91310381/cb1b7467-bf72-41df-b66c-cd2f4a607e58)

根据店铺管理员管理店铺信息的时序图可以创建如下协作图:

![13](https://github.com/curryluku/SE_Final-Paper/assets/91310381/9fa76b04-ea64-4248-87d5-614f1b4c30c4)

## 5.1.4 店铺管理员建立客户评价档案

(1)店铺管理员登录到系统:

(2)对订餐者的评价进行核实并筛选:

(3)生成最终的评价档案:

(4)系统将结果显示给店铺管理员:

(5)退出系统。

![14](https://github.com/curryluku/SE_Final-Paper/assets/91310381/9f05b15d-19cd-4342-8b4b-2e029dad593c)

根据店铺管理员建立客户评价档案的时序图可以创建如下协作图:

![15](https://github.com/curryluku/SE_Final-Paper/assets/91310381/65cd17b3-b6f8-4951-af41-5bfac60045e7)

## 5.1.5 店铺管理员建立商家监察档案

(1)店铺管理员登录到系统:

(2)录入通过检查得出的监察结果:

(3)生成监察档案:

(4)系统将结果显示给店铺管理员:

(5)退出系统。

![16](https://github.com/curryluku/SE_Final-Paper/assets/91310381/4b4fd71c-4092-45c8-946c-07f986bc29aa)

根据店铺管理员建立商家监察档案的时序图可以创建如下协作图:

![17](https://github.com/curryluku/SE_Final-Paper/assets/91310381/d0d160be-3b7c-4811-9c35-ddf4b551d0e7)

## 5.1.6 订单管理员管理订单

(1)订单管理员登录到系统中:

(2)管理订单信息:

(3)提交更新数据:

(4)系统将更新结果显示给定单管理员:

(5)提交成功,退出系统。

![18](https://github.com/curryluku/SE_Final-Paper/assets/91310381/b143a6c6-2d41-4754-82ba-3f07531edcb9)

根据订单管理员管理订单的时序图可以创建如下协作图:

![19](https://github.com/curryluku/SE_Final-Paper/assets/91310381/c37c5ded-37e4-41f8-bdc6-e3068429ee2c)

## 5.1.7 系统管理员管理订餐者信息

(1)系统管理员注册一个自己的登录账号:

(2)输入用户名和密码进行身份验证:

(3)系统将验证结果显示结果返回给系统管理员:

(4)系统管理员在订餐者信息管理界面对订餐者信息进行更新:

(5)提交更新数据:

(6)系统将提交结果返回:

(7)提交成功,退出系统。

![20](https://github.com/curryluku/SE_Final-Paper/assets/91310381/66cb8d7a-41a8-48a2-b74a-9c265d351791)

根据系統管理员管理订餐者信息的时序图可以创建如下协作图:

![21](https://github.com/curryluku/SE_Final-Paper/assets/91310381/b3441386-0b9f-4c8a-871f-a0966ff3aa30)

## 5.1.8 系统管理员管理商家信息

(1)系统管理员注册一个自己的登录账号:

(2)输入用户名和密码进行身份验证:

(3)系统将验证结果显示结果返回给系统管理员:

(4)系统管理员在商家信息管理界面对商家信息进行更新:

(5) 提交更新数据:

(6)系统将提交结果返回:

(7)提交成功,退出系统。

![22](https://github.com/curryluku/SE_Final-Paper/assets/91310381/3aa9b993-f7af-43bd-9263-54c24fa8edff)

根据系统管理员管理商家信息的时序图可以创建如下协作图:

![23](https://github.com/curryluku/SE_Final-Paper/assets/91310381/1f204173-a0d4-436e-81d6-79cf6666ad2a)

## 5.1.9 系统管理员维护系统

(1)系统管理员注册一个自己的登录账号:

(2)输入用户名和密码进行身份验证:

(3)系统将验证结果显示结果返回给系统管理员:

(4)系统管理员在系统维护界面对系统进行维护:

(5)提交维护操作:

(6)系统将提交结果返回:

(7)提交成功,退出系统。

![24](https://github.com/curryluku/SE_Final-Paper/assets/91310381/1394dbbe-9599-4de2-9ec3-022af1c02b2c)

根据系统管理员维护系统的时序图可以创建如下协作图:

![25](https://github.com/curryluku/SE_Final-Paper/assets/91310381/08150eb3-8c48-441e-93ac-999e6a3a3dbb)

## 5.2 系统活动图

根据大学生网上订餐系统的整个活动过程,创建了如下的系统活动图:

![26](https://github.com/curryluku/SE_Final-Paper/assets/91310381/521faeb6-4649-4882-8487-f01e8df5a835)

## 5.3 系统状态图

根据前面的分析和设计可以发现,每个参与者在使用系统前都需要进行登录,登录之后就可以进行各自相应的操作,操作完成后退出系统。创建的系统状态图如下:

![27](https://github.com/curryluku/SE_Final-Paper/assets/91310381/064534f4-edf2-4977-abb5-75ea9485ce25)

# 6.系统部署图

## 6.1 系统构件图

网上订餐系统的构件图我们通过构件映射到系统的实现类中, 说明该构件物理实现的逻辑类,在本系统中,我们可以对订餐者类、系统管理员类、商家类、店铺管理员类、订单管理员类、订单类和餐饮类分别创建对应的构件进行映射。

![28](https://github.com/curryluku/SE_Final-Paper/assets/91310381/e817539d-3578-4492-8321-e3a30edec7ee)

## 6.2 系统部署图

网上订餐系统的部署图描绘的是系统节点上运行资源的安排。包括四个节点,分别是:客户端浏览器、HTTP服务器、数据库服务器和打印机。

![29](https://github.com/curryluku/SE_Final-Paper/assets/91310381/a6cb859b-0fdf-461d-aac1-50af2313f770)

# 7.总结

经过认真地分析我得出了系统的需求分析,确定了系统的主要参与者以及各自的主要活动。通过学习 UML建模的有关知识和 Rational Rose工具,我亲自动手练习,最终画出了系统的系统用例模型(各自用例的用例图)、系统静态模型 (系统类图)、系统的动态模型(系统时序图、系统活动图和系统状态图)以及系统部署模型(系统构件图和系统部署图)。通过自己的亲自动手操作,使我进一步了解并掌握了 UML的建模过程和 Rational Rose工具的使用。同时,我也发现了自己思考问题不全面等一系列不足,促使自己不断改正、不断进步。
