# Discover IntelliJ IDEA

本指南旨在帮助您通过IntelliJ IDEA提高工作效率，并提供最重要功能的概述，提示，技巧和最热门的快捷方式。

## User interface

IntelliJ IDEA编辑器在很多方面都很特别，最值得注意的是你可以在不离开的情况下调用几乎任何IDE功能，这允许你组织一个有更多屏幕空间的布局，因为隐藏了工具栏和窗口之类的辅助控件。

![refcard 1](https://www.jetbrains.com/help/img/idea/2018.2/refcard_1.png)

通过快捷方式访问工具窗口会将输入焦点移动到它，因此您可以在其上下文中使用所有键盘命令。 当您需要返回编辑器时，请按Escape。

下面是调用您最常需要的工具窗口的快捷方式列表：

| Tool Window     | Shortcut |
| --------------- | -------- |
| Project         | Alt+1    |
| Version Control | Alt+9    |
| Run             | Alt+4    |
| Debug           | Alt+5    |
| Terminal        | Alt+F12  |
| Editor          | Escape   |

如果您不知道某个操作的快捷方式，请按Ctrl + Shift + A尝试使用“查找”操作功能。 开始键入以按名称查找操作，查看其快捷方式或调用它。

如果您想专注于代码，请尝试无牵引模式。 它会删除所有工具栏，工具窗口和编辑器选项卡。 要切换到此模式，请在主菜单上选择 View | Enter Distraction Free Mode.

“无牵引模式”的替代方法可能是按Ctrl + Shift + F12隐藏所有工具窗口。 您可以再次按此快捷方式将布局恢复为默认值。

导航栏是项目工具窗口的紧凑替代品。 要访问导航栏，请按Alt + Home。

![refcard 2](https://www.jetbrains.com/help/img/idea/2018.2/refcard_2.png)

IntelliJ IDEA中的大多数组件（工具窗口和弹出窗口）都提供速度搜索。 此功能允许您过滤列表，或使用搜索查询导航到特定项目。

![refcard 7](https://www.jetbrains.com/help/img/idea/2018.2/refcard_7.png)

有关详细信息，请参阅周围的导览 [Guided Tour around the User Interface](https://www.jetbrains.com/help/idea/guided-tour-around-the-user-interface.html), [Editor basics](https://www.jetbrains.com/help/idea/using-code-editor.html)和[Working with Tool Windows](https://www.jetbrains.com/help/idea/tool-windows.html).

# Guided Tour around the User Interface

在这里，您可以了解IntelliJ IDEA用户界面的组织方式，以帮助您找到适合您工作环境的方法。

当您第一次运行IntelliJ IDEA或没有打开项目时，IntelliJ IDEA会显示欢迎屏幕，可以快速访问主要入口点。 打开项目时，IntelliJ IDEA将显示主窗口。

IntelliJ IDEA的主窗口由逻辑区域组成，如下图所示，标有数字标签：

![large mainWindow](https://www.jetbrains.com/help/img/idea/2018.2/large_mainWindow.png)

1. **Main menu and toolbar**  包含影响整个项目或大部分项目的命令，例如打开，创建项目，重构代码，运行和调试应用程序，保持文件受版本控制等等。

   主工具栏复制主菜单的基本命令，以便更快地访问。 默认情况下，主工具栏是隐藏的。 要显示它，请选择**View | Toolbar**的工具栏。

2. **Navigation bar** 有关更多详细信息，请参阅 [用户界面](https://www.jetbrains.com/help/idea/guided-tour-around-the-user-interface.html)， [编辑器基础知识](https://www.jetbrains.com/help/idea/using-code-editor.html)和[使用工具Windows的](https://www.jetbrains.com/help/idea/tool-windows.html)[导览](https://www.jetbrains.com/help/idea/guided-tour-around-the-user-interface.html)。

   使用**View | Navigation Bar** 隐藏或显示导航栏; 按**Alt + Home**将应用程序焦点置于导航栏。

3. **Status bar** 表示项目的状态，整个IDE，并显示各种警告和信息消息。

4. **Editor**   在这里，您可以阅读，创建和修改代码。

5. **Tool windows**  辅助窗口，提供对各种特定任务的访问（项目管理，搜索，运行和调试，与版本控制系统集成等）。

# Configuring Project and IDE Settings

在IntelliJ IDEA中，您可以在两个级别（项目级别和IDE级别）上配置设置和结构。

## Project-level settings and structure

项目级别设置和结构仅应用于当前项目。 这些设置与.idea目录中的其他项目文件一起存储。

如果您的项目受版本控制，建议在版本控制下存储具有项目特定设置的XML文件（项目文件夹中的.idea文件夹），例外是workspace.xml和tasks.xml，它们存储用户 - 具体设置。

您可以在GitHub上参考这个JetBrains.gitignore来查看应该忽略的内容。

```ini
# Covers JetBrains IDEs: IntelliJ, RubyMine, PhpStorm, AppCode, PyCharm, CLion, Android Studio and WebStorm
# Reference: https://intellij-support.jetbrains.com/hc/en-us/articles/206544839

# User-specific stuff
.idea/**/workspace.xml
.idea/**/tasks.xml
.idea/**/usage.statistics.xml
.idea/**/dictionaries
.idea/**/shelf

# Generated files
.idea/**/contentModel.xml

# Sensitive or high-churn files
.idea/**/dataSources/
.idea/**/dataSources.ids
.idea/**/dataSources.local.xml
.idea/**/sqlDataSources.xml
.idea/**/dynamic.xml
.idea/**/uiDesigner.xml
.idea/**/dbnavigator.xml

# Gradle
.idea/**/gradle.xml
.idea/**/libraries

# Gradle and Maven with auto-import
# When using Gradle or Maven with auto-import, you should exclude module files,
# since they will be recreated, and may cause churn.  Uncomment if using
# auto-import.
# .idea/modules.xml
# .idea/*.iml
# .idea/modules

# CMake
cmake-build-*/

# Mongo Explorer plugin
.idea/**/mongoSettings.xml

# File-based project format
*.iws

# IntelliJ
out/

# mpeltonen/sbt-idea plugin
.idea_modules/

# JIRA plugin
atlassian-ide-plugin.xml

# Cursive Clojure plugin
.idea/replstate.xml

# Crashlytics plugin (for Android Studio and IntelliJ)
com_crashlytics_export_strings.xml
crashlytics.properties
crashlytics-build.properties
fabric.properties

# Editor-based Rest Client
.idea/httpRequests

# Android studio 3.1+ serialized cache file
.idea/caches/build_file_checksums.ser
```

Global/JetBrains.gitignore

## Access the project-level settings

在window和Linux中选择 **File | Project Structure** .