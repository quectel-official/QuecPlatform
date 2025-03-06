[English](https://github.com/quectel-official/QuecPlatform/blob/main/vscode-extension/md/README.md) | 中文

# QuecPlatform for VSCode

Quectel OpenCPU一站式开发平台。🚀

## 特性

> ✅ 支持多款模组<br>
> ✅ 支持CSDK开发 <br>
> ✅ 支持代码一键拉取、编译、烧录 <br>
> ✅ 支持Windows/Linux开发 <br>

## 快速入门

1. 在VSCode商店中安装`QuecPlatform`插件。
2. 点击'`Q`'图标打开插件并等待其加载完毕。<br>
![first page](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/first_page.png)
3. 在左侧菜单栏你将会看到如下几个按钮: 
    - `Home`: 主页。在这里你可以创建新工程、打开一个已存在的工程、查看所有平台包、查看已安装的平台所支持的开发板包。

    - `Create project`: 创建新工程。点击该按钮将会弹出选择目标板的选项，如果提示“No package has been downloaded, please download the package first”，则表示你没有下载任何平台或开发板包。你需要先去`Home`下载它：
      - 如果你看到这个提示则说明你需要先下载一个开发板包。<br>
        ![no package](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/no_package.png)
        1. 前往`Home`界面。
        2. 安装一个平台包，如果你之前没有安装过。<br>
        ![install platform](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/install_platform.png)
        3. 安装一个开发板包，例如`FC41D`。 `下载开发板包前请确保你已在Home界面Account栏中输入了正确的用户名和访问令牌（见第四节：访问令牌获取）`。<br>
        ![install board](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/install_board.png)
        4. 等待开发板包安装完成。
        
    - `Open project`: 打开一个已存在的工程。

    - `Conversion project`: 将工具不支持的工程转换为工具所支持的工程。由于一站式编译的需要，该工具仅支持特定的项目，但是您可以使用此选项将工具不支持的工程转换为工具所支持的工程，但仅适用于工具支持的开发板。

    - `Build`: 如果您已经创建或打开了一个工程，您可以点击此按钮进行编译，如果没有打开的工程，请参照上面的步骤创建或打开一个。

    - `Upload`: 烧录固件。烧录前请确保选择了正确的端口。

    - `Restart QuecPlatform`: 重启插件，如果插件没有正常工作。

4. 访问令牌获取
   - 安装Quectel的开发板包前需要获取到GitLab的访问令牌才能进行代码拉取。

   - 左侧输入框是你GitLab账号的用户名，右侧是你的访问令牌，下面是更改按钮，点击它账号就可以生效，下面将介绍如何申请访问令牌。<br>
    ![set account](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/set_account.png) 

   - 登录你的GitLab账号，鼠标左键单击你的头像，然后在选项中选择`preferences`进入设置界面。 <br>
    ![goto setting](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/goto_setting.png)

   - 在左侧菜单栏找到`Access Tokens`选项，然后点击`Add new token`按钮创建新的访问令牌，如果之前没有的话。<br>
    ![get account1](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/get_account1.png) 

   - 在如下界面输入：`Token name`，token名称，可自由填写；`Expiration date`，截止日期，你可以根据实际需要选择长一点的；最后是token权限，请根据实际需求勾选权限，作为测试的话你可以全部勾选，最后点击`Create`按钮完成创建。<br>
    ![get account2](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/get_account2.png) 

   - 最后复制生成的访问令牌，并填入`Home`界面Account栏中的指定位置。

5. 你可以在底部状态栏中看到如下几个按钮：<br>
    ![status bar](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/status_bar.png)
    - `o` 编译按钮。
    - `√` 烧录按钮。
    - `d:/0_work/prjs/FCM360W_TEST` 当前的工程，你可以点击这里来切换工程。
    - `COM1` 当前选择的端口号，你可以点击这里来切换端口号。

## 版本历史

### 0.1.2
-------------------------
- 在Home界面添加快速入门文档入口；
- 新增工程转换功能，支持将工具不支持的工程转换为工具所支持的工程；
- 修复已知问题。


### 0.1.1
-------------------------

- 第一个BETA版本。

## 更多信息

Quectel: https://www.quectel.com.cn/

Quectel - Short Range: https://short-range.quectel.com/
