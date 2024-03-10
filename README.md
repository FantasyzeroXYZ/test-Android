# Android待办事项
* [ ] 

# test-Android
* 环境搭建
  * JDK
  * Android SDK
  * Android studio 
    * 下载 https://developer.android.com/studio?hl=zh-cn
    * 安装
    * 插件
      * 界面汉化
        1. 查看安装的Android studio版本再选择对应的中文语言包下载
          * 确定Android studio版本
            * Help->About
            * 查看Build#AI前三位
          * 选择对应的中文语言包
            * 中文语言包 https://plugins.jetbrains.com/plugin/13710-chinese-simplified-language-pack----
            * 将Android studio里查看到的Build#AI前三位在页面进行`ctrl+F`搜索
        2. 安装下载好的中文语言包
          * File(文件)->Settings(设置)
          * Plugins(插件)->install Plugin form Disk(从磁盘安装插件)
          * 在路径里选择下载好的中文语言包
        3. 重启Android studio
        * 取消汉化
          1. 文件->设置->插件
          2. 取消勾选汉化插件
          3. 应用，重新启动IDE 
    * [ ] 配置git
      * Version control(版本控制)
      * (设置)->github
      * (设置)->git
      * 提交到现有仓库
      * 新建仓库
      * 退出GitHub账号
    * [ ] 创建新项目
    * [ ] 构建
    * [ ] Run/Debug Configurations(运行/调试配置)？
    * [ ] 实时预览
      * 项目文件app->src->main->res->layout下的xml文件
    * [ ] Android studio卡顿解决方案
    * [ ] Design editor is unavailable until after a successful project sync？
    * Gradle
      * 配置国内镜像
        * 项目文件gradle->wrapper->gradle-wrapper.properties
        * 替换`distributionUrl=`后面的内容
          * 将`https\://services.gradle.org/distributions/`替换成`https://mirrors.cloud.tencent.com/gradle/`
      * [ ] 下载对应版本替换
        * 官方下载 https://services.gradle.org/distributions/
        * 国内镜像下载 https://mirrors.cloud.tencent.com/gradle/
    * [ ] 可视化添加
      * 打开实时预览
* Android studio练习
  * [ ] 理清项目文件结构
  * 在button的xml中增加`android:gravity="center"`即可实现文字水平居中
  * 更改button背景颜色`android:backgroundTint="@android:color/background_dark"`
  * [ ] 参考 https://blog.csdn.net/nuanpang/article/details/125847905
  * xml布局
    * Button
    * EditText
    * TextView
  * 插入图片
* vscode插件
* 网站
* kotlin
  * 官网 https://kotlinlang.org/
  * 想使用Kotlin必须安装JDK
  * 下载kotlin编译器 https://github.com/JetBrains/kotlin/releases
  * 配置环境变量
    * KOTLIN_HOME 文件所在路径
    * 在Path里添加%KOTLIN_HOME%\bin
  * vscode插件
    * Code Runner
    * Kotlin Language
  * 测试配置是否已完成
    * `kotlinc -version`
  * 设置code-runner在终端运行命令
    * 在设置里搜索code-runner.runInTerminal并勾选上
  * 配置jupyter
    * https://github.com/Kotlin/kotlin-jupyter
    * 创建虚拟环境`pipenv install`
    * 安装kotlin-jupyter-kernel`pipenv install kotlin-jupyter-kernel`
    * 创建ipynb文件并选择kotlin内核