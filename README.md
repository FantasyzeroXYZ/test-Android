# Android待办事项
* [ ] 

# 资源待整理
* 关键词
	* Android studio
* Awesome Android https://github.com/JStumpp/awesome-android
* 安卓面试
  * Awesome-Android-Interview https://github.com/JsonChao/Awesome-Android-Interview
* UI库
  * awesome-github-android-ui https://github.com/opendigg/awesome-github-android-ui
  * List of Android UI/UX Libraries https://github.com/wasabeef/awesome-android-ui
* Android Studio插件
  * Android Studio Plugins https://github.com/balsikandar/Android-Studio-Plugins
  * Android Studio插件 https://github.com/szqcharles/Android-Studio-Plugins-cn
  * TranslationPlugin（IDE文档翻译插件） https://github.com/YiiGuxing/TranslationPlugin
# test-Android
* kotlin
  * 官网 https://kotlinlang.org/
  * 想使用Kotlin必须安装JDK
  * 下载kotlin编译器 https://github.com/JetBrains/kotlin/releases
  * 在线运行代码 https://play.kotlinlang.org/
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
    * 关于git版本管理 
      * [ ] 配置git
        * Settings(设置)->Version control(版本控制)->Git
      * [ ] Github
        * Settings(设置)->Version control(版本控制)->GitHub
        * 在Android studio里授权登录GitHub
          1. 左上角`Version control`->Share Project On->github或者
          2. 登录github进行授权
          3. 提交到仓库
             * 新建仓库
             * 现有仓库提交方式？
        * [ ] 退出GitHub账号
          1. File->Setting
          2. Version Control->github或者直接在搜索栏搜索`github`
          3. 选择账户进行移除
      * [ ] gitee
        * [ ] 安装gitee插件
          * https://plugins.jetbrains.com/plugin/11491-gitee
        * Settings(设置)->Version control(版本控制)->Gitee
    * Gradle
      * 配置国内镜像
        * 项目文件gradle->wrapper->gradle-wrapper.properties
        * 替换`distributionUrl=`后面的内容
          * 将`https\://services.gradle.org/distributions/`替换成`https://mirrors.cloud.tencent.com/gradle/`
      * [ ] 使用本地gradle的配置
        * 下载对应版本替换
          * 官方下载 https://services.gradle.org/distributions/
          * 国内镜像下载 https://mirrors.cloud.tencent.com/gradle/

* Android调试
  * [ ] 云真机
  * [ ] Android studio模拟调试
  * [ ] 本地真机调试


# 其他待整理
* 创建新项目
  * File->New->New Project
  * 选择相应的Activity
  * 或者选择`No Activity`自行创建Activity
* [ ] 导入/打开项目
  * File->open
* [ ] 构建
* [ ] Run/Debug Configurations(运行/调试配置)？
* [ ] Android studio卡顿解决方案
* [ ] Design editor is unavailable until after a successful project sync？

* gitee
  * 创建分支
    * 分支起点
  * [ ] 克隆分支
    * `git clone -b 分支名 仓库URL`
  * [ ] 推送分支
    * `git push -u 远程仓库的别名 本地分支名称:远程分支名称`
  * 查看当前分支`git branch`
  * 配置
    * `ssh-keygen -t rsa -f C:/Users/用户名/.ssh/id_rsa_gitee -C "邮箱"`
    * `ssh-keygen -t rsa -f C:/Users/10352/.ssh/id_rsa_gitee -C "1035203852@qq.com"`
    * `ssh-keygen -t ed25519 -f C:/Users/10352/.ssh/id_ed25519_github -C "fantasyzeroxyz@gmail.com"`
  * 清除账户全局配置
    * `git config --global --unset user.name "用户名"`
      * `git config --global --unset user.name "FantasyzeroXYZ"`
    * `git config --global --unset user.email "用户邮箱"`
      * `git config --global --unset user.email "fantasyzeroxyz@gmail.com"`
  * 让SSH识别新的私钥
    * 移动到.ssh目录下
    * 输入如下命令
      * `ssh-agent bash`
      * `ssh-add .\id_ed25519_github`
      * `ssh-add .\id_rsa_gitee`
  * 配置.ssh里的config文件
    * 添加上一行`IdentityFile 对应私钥文件地址`
      * `IdentityFile ~/.ssh/id_ed25519_github`
  * 查看私钥pub文件内容添加到相应网站
    * `cat 私钥pub文件`
      * `cat .\id_rsa_gitee.pub`
  * 测试是否连接成功
    * `ssh -T -p 443 git@ssh.github.com`
    * `ssh -T git@ssh.gitee.com`
  * 单独对仓库设置账号
    * 在仓库目录下`cd .git`
    * `git config user.name 'CrazyNPC'`
    * `git config user.email '1035203852@qq.com'`
  * `git config -l`查看 按q退出
  * 编辑配置`git config --edit`

* 界面设计
  * 布局(xml布局文件)
    * 类型
      * 线性布局LinearLayout
        * 位置由水平或垂直方向依次排列
      * 相对布局RelativeLayout
        * 可以自由放置
      * 约束布局ConstraintLayout
        * 可以添加引导线（Guideline）来辅助布局，所有的布局可以在如图所示的界面上通过拖动和调整来完成，相对于RelativeLayout这一点要方便许多
    * 方式
      * 实时预览
        * 项目文件app->src->main->res下的xml布局文件
  * 控件
    * Button
    * EditText
    * TextView
    * 插入图片

* Android studio练习
  * [ ] 理清项目文件结构
  * 在button的xml中增加`android:gravity="center"`即可实现文字水平居中
  * 更改button背景颜色`android:backgroundTint="@android:color/background_dark"`
  * [ ] 参考 https://blog.csdn.net/nuanpang/article/details/125847905
  
# Android studio 
* 1
  * 创建Activity
  * 创建布局文件xml
    * 放置组件
      * button
        * https://blog.csdn.net/pan2635376816/article/details/116789912
  * 在Activity里加载布局
    * setContentView(R.layout.布局文件名称)
  * `android:exported="true"`
  * 添加<intent-filter>的内容设置主Activity
    ```
    <activity
        android:name=".MainActivity"
        android:exported="true">
        <intent-filter>
            <action android:name="android.intent.action.MAIN"/>
            <category android:name="android.intent.category.LAUNCHER" />
        </intent-filter>
    </activity>
    ```
  * 控件
    * textview文本内容输入
      * android:text="输入文本内容"
    * imageview
      * 设置图片显示
        * android:src="@res文件夹下的对应图片路径"
      * 图片导入
    * drawable或mipmap文件夹存放图片的区