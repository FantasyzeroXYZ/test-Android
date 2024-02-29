# Android待办事项
* [ ] 

# test-Android
* 环境搭建
  * JDK
  * Android SDK
  * Android studio 
    * 下载 https://developer.android.com/studio?hl=zh-cn
    * 安装
    * 配置
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
    * [ ] 配置git
      * Version control(版本控制)
      * (设置)->github
      * (设置)->git
      * 提交到现有仓库
      * 新建仓库
      * 退出GitHub账号
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