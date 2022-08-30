LabVIEW-UI-ProcessDlg
===========================

LabVIEW 使用的进度对话框，用于忙碌时指示程序工作状态。

**忙碌模式(Buzy Window)**   
![忙碌模式](https://images.gitee.com/uploads/images/2018/1008/153055_08c8feaa_136753.png "屏幕截图.png")

**进度条模式(Progress Window)**   
![进度条模式](https://images.gitee.com/uploads/images/2018/1008/153124_5be7aa2a_136753.png "屏幕截图.png")

**计时器模式(Timer Window)**   
![计时器模式](https://images.gitee.com/uploads/images/2018/1008/152916_a3972e16_136753.png "屏幕截图.png")

调用方法
---------------

### 调用流程

![输入图片说明](https://images.gitee.com/uploads/images/2018/1008/153714_91320bc1_136753.png "屏幕截图.png")

 1. 初始化，成功后进度条对话框将弹出;
 2. 根据需要设置界面属性
    - 设置窗口Title;
    - 设置窗口是否可以关闭；
    - 设置进度条状态；
    - 重置计时;
    - etc...
 3. (Optional)在窗口是否可以关闭的情况下，通过 Get Stopped.vi 或 Stop User Event 获取停止状态
 4. 释放进度条资源，关闭窗口

### 开发环境
LabVIEW 2014

### 依赖项
 - N/A
 
修改记录
---------------
 - V1.0 创建项目
 - V2.0 
    - 增加计时器模式
    - 增加窗口的关闭选项，可以通过 Get Stopped.vi 或 Stop User Event 获取停止状态
    - 窗口居中显示在UI窗口位置
