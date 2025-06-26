# Overiew
This repo will including all basic knowledge of VScode. 
- README file will document all details
- sample code for tesing on local
# VScode
VS Code is a workspace which collected one or more folders. Most of the time, having a single folder opened as the workspace. VScode is not a IDE, is a text editor.

Visual Studio Code is a free, lightweight, and extensible code editor for building web, desktop, and mobile applications, using any programming language and framework.

Visual Studio Code has built-in support for Git source control management and powerful integrations with GitHub, an integrated debugger, and smart code completion with IntelliSense and with AI-driven IntelliCode. With over 30,000 extensions and themes in the Visual Studio Code Marketplace, you can customize the features and the look of Visual Studio Code to fit your needs, preferences, and style.

You can use Visual Studio Code to build any kind of app, for web, desktop, and mobile. Visual Studio Code supports JavaScript and TypeScript natively and offers extensions for coding in languages such as Python, Java, C/C++, C#, Go, Rust, PHP, and many more.

-[Reference Link](https://apps.microsoft.com/detail/xp9khm4bk9fz7q?hl=en-US&gl=US)

## VScode Install
[Download Link](https://code.visualstudio.com/download)

## .vscode/ folder
.vscode/ folder is used to store workspace-specific settings. likes:
- `settings.json` project specific settings. 
- `launch.json` debug configuration
- `tasks.json` shared tasks and build commands
- `extensions.json` project specific extensions in
### how to set up/modify the setting
- Press `F1` or `go to ->view->command palette` or `Ctrl+Shift+P`
- type `user settings` and select `Preferences: Open User Settings`
- Settings will open
- 2 types of settings, User or Workspace
    - User setting : global settings.json file and is applied to all projects(workspaces) of the current user.
    - Workspace: setting written to your `.vscode/seetings.json` file 
### Should commit .vsccode directory to scource control
Depending on what you want to share or not to team members.




## VScode/Java
### Java Conigure
1. Install JDK: needs 1.8+
2. Install Extensions: Language Support for Java™ by Red Hat
3. Create a Project
4. Start your coding now
- [Java Extension List](https://code.visualstudio.com/docs/java/extensions)

### Java/Maven Configure
1. Install JDK: JDK11 or higher, using `java -version` to check the version
2. Install Maven: using `mvn -version` to check.
3. Install Extensions:
    * Java Extension Pack
    * Maven for Java
4. Create a Maven Project in VScode
    - Open Command Palette: go View-> Command Palette
    - Select Maven: Create Maven Project
    - Select Archetype: maven-archetype-quickstart and version 1.0
    - Enter Group Id
    - Enter Artifiact ID
    - Choose a Location: the place where to save the project
    - Adding Dependencies to the Project: modify pom.xml
    - start your coding now
    - click run button on the top-right corner of the editor
    - output will appear in the Terminal or Debug Console
5. Create a Maven project in Terminal
    - cd to your location
    - run `mvn archetype:generate -DgroupId=com.example -DartifactId=my-maven-project -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false`
    - check the folder structer after build success
    - open floder on VScode
    - Adding Dependencies to the Project: modify pom.xml
    - start your coding now
    - cd to pom.xml located
    - run `mvn compile` to compile the project
    - run `mvn exec:java -Dexec.mainClass="com.example.App"` to execute the code
    - output should display now

* [mavenSearch](https://mvnrepository.com/) : e.g:input `testNg` on search field.

Troubleshooting:
- Maven not Recognized: check Maven was added to systme Path
- Dependency Issues: check the pom.xml file
- Slow intelliSense: Restart VScode or disable unnecessary extensions

## VScode/Python

## VScode/Robot/Python

## VScode/C/C++

## VScode/C#

