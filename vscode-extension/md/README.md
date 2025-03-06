English | [中文](https://github.com/quectel-official/QuecPlatform/blob/main/vscode-extension/md/README_CN.md)

# QuecPlatform for VSCode

This is the OpenCPU development platform developed by Quectel.🚀

## Features

> ✅ Suitable for multiple modules <br>
> ✅ Support CSDK development <br>
> ✅ Supports one-click clone, compile and download <br>
> ✅ Supports Windows and Linux <br>

## Quick Start

1. Install the `QuecPlatform` extension in the VSCode marketplace.
2. Click the 'Q' icon to open the plugin and wait for it to load.<br>
![first page](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/first_page.png)
3. In the left menu bar you will see the following buttons: 
    - `Home`: home page. Here you can create a new project, open an existing project, view all platform packages, and view board packages supported by installed platforms.

    - `Create project`:  Creates a new project. Clicking this button will bring up the option to select the target board. If the message `No package has been downloaded, please download the package first` is displayed, it means that you have not downloaded any platform or development board package. You need to go to `Home` to download it first:
      - If you see this prompt, it means you need to download a board package first.<br>
        ![no package](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/no_package.png)
        1. Goto the `Home` page.
        2. Install a platform package if you haven't installed it before.<br>
        ![install platform](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/install_platform.png)
        3. Install a board package, for example, FC41D. `Please ensure that you have entered the correct user name and access token in the Account field of the Home screen before downloading the development board package (See Section 4: Access Token Acquisition)`. <br>
        ![install board](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/install_board.png)
        4. Wait until the development board package is installed.
        
    - `Open project`: Open an existing project.

    - `Conversion project`: Convert project not supported by the tool to the project supported by the tool. Due to the need for one-stop compilation, the tool only supports specific projects, but you can use this option to convert unsupported projects to supported projects, but only for the boards supported by the tool.

    - `Build`: If you have already created or opened a project, you can click this button to compile, if there is no open project, please follow the steps above to create or open one.

    - `Upload`: To burn firmware, please select the correct serial port before burning.

    - `Restart QuecPlatform`: Restart the extension, when it doesn't work well.

4. Access Token Acquisition
   - Before installing Quectel's board package, you need to obtain an access token from GitLab for code pulling.

   - The left input box is the user name of your GitLab account, the right is your access token, below is the change button, click on it account can take effect, the following will explain how to apply for access token. <br>
    ![set account](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/set_account.png) 

   - Log in to your GitLab account, left click on your avatar, and then select `preferences` from the options to enter the Settings screen.<br>
    ![goto setting](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/goto_setting.png)

   - Find the `Access Tokens` option in the left menu bar and click on the `Add new token` button to create a new access token if you did not have one before.<br>
    ![get account1](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/get_account1.png) 

   - Enter `Token name`, which can be filled freely; `Expiration date`, you can choose a longer expiration date according to the actual need; The last is the token permissions, please check the permissions according to the actual needs, as a test you can check all, and finally click the `Create` button to complete the creation. <br>
    ![get account2](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/get_account2.png) 

   - Finally copy the generated access token and fill it in the specified location in the Account field of the `Home` page.

5. You can see the following buttons in the bottom status bar:<br>
    ![status bar](https://raw.githubusercontent.com/quectel-official/QuecPlatform/main/vscode-extension/md/status_bar.png)
    - `o` build button.
    - `√` upload button.
    - `d:/0_work/prjs/FCM360W_TEST` the current project, you can click here to switch the project.
    - `COM1` the currently selected port number, you can click here to switch the port number.

## Release Notes

### 0.1.2
-------------------------
- Add a quick start document entry to the home page.
- Added the Project conversion function, which can convert the project not supported by the tool to the project supported by the tool;
- Fix known issues.


### 0.1.1
-------------------------
- The first beta version.


## For more information

Quectel: https://www.quectel.com.cn/

Quectel - Short Range: https://short-range.quectel.com/
