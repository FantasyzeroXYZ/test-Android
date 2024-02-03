# test-Android
* 环境搭建
  * JDK
  * Android SDK
  * Android studio 
    * 下载 https://developer.android.com/studio?hl=zh-cn
    * 安装
    * 配置
    * 插件
      * 汉化
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