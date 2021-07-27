# 每日精选
## 整体框架
1、首先导入资源对象，调整相应的位置，属性等。  
2、编写脚本读取json，并且给相应的组件编写事件    
3、绑定脚本与游戏对象  
4、运行测试程序  
## 目录结构
Assets
>> Materials  
>> Prefabs  
>> Scenes  
>> Scripts  
>> Images  
## 界面结构拆分
### Hierarchy层
> MainScenes 场景 
> 
> Background
>> Image  
> Labels
>> 金币信息位置
>> TitleLables 2个(每日精选一个，士兵招募一个)  
>>  MainLable 2个
>>> DayCardsBgLable 每日精选1个
>>>> CardBackgroundLab 每日精选宝箱位3n个
>>>>> BuyButton 购买按钮
>>>>>> img 金币 对号  
>>>>>> Text 价格 已购买   
>>>>> img 宝箱图片  
>>>>> titleText 名称   
>>> SoldiersBgLable 士兵招募1个   
>>>> SoldBackgroundLab 士兵招募1个  
### Prefab 预制件
> 3个Prefab
>> 已解锁宝箱1个    
>> 未解锁宝箱1个    
>> 购买按钮1个  
## 代码结构
> 3个脚本文件  
>> MainSceneController 主场景控制器  
>>> StartSceneView 场景初始化方法  
>>> SceneChangeView 场景切换方法  
>>> QuitSceneView 退出场景  
>> GameObjectEvent 游戏事件类  
>>> ButtonClick 按钮点击方法   
>>> AlreadyBuy 宝箱已购买方法    
>>> ReadyBuy 宝箱未购买方法  
## 流程图
# 下面是赋值语句
st=>start: Start|past:>http://www.google.com[blank]
e=>end: End:>http://www.google.com
op1=>operation: My Operation|past
op2=>operation: Stuff
cond=>condition: Yes or No?
c2=>condition: Good idea
io=>inputoutput: catch something...

# 下面是连接语句
st->op1->cond
cond(yes)->c2
c2(yes)->io->e
c2(no)->op2->e

