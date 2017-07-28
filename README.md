# yuLearnNote
在有鱼互娱的笔记
在游戏中需要创建一个页面的步骤
资源部分：
1.复制一个以前的页面  path : res/res_mk/UI/Resources 找一个类似的
2.用cocos builder 打开项目 
3.修改完成  点击 cocos builder 中的 File -> publish 保存

代码部分：
1.在相应的地方添加lua代码  如：创建了一个叫 BeibaoItemTest.ccb 的文件， 就在项目中添加一个BeibaoItemTest.lua文件 (此处不要忘记了，把复制的其它.lua文件的方法的名称也修改了)
2.在ui代码部分   script_useless -> UI -> core -> ccLoader.lua 中 添加BeibaoItemTest的相关引用 
1.require "创建的.lua文件"
2.kCCB_**   --复制出来的.ccb文件
3.在ccbClassMap 的table 中添加  .lua 中的class 名  如BeibaoItemTest.lua 的中class 叫BeibaoItemTest 

#主页面  ：mainPanel.lua 
#网络请求： 都在common  -> controller 中
---------------------------------------------------------------------------
