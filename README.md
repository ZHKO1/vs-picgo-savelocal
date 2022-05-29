# vs-picgo-savelocal

> 基于vs-picgo新增保存图片到本地的插件，更好地管理markdown里图片资源。

## Overview
 和 [vs-picgo](https://github.com/PicGo/PicGo-Core) 保持一致，唯一的不同是新增了picgo.localSavePath配置，可以根据md文件名自由配置本地保存地址

## Features

<details>
<summary>Uploading an image from clipboard</summary>
<img src="https://i.loli.net/2019/04/09/5cac17d2d2265.gif" alt="clipboard.gif">
</details>

<details>
<summary>Uploading images from explorer</summary>
<img src="https://i.loli.net/2019/04/09/5cac17eea0d65.gif" alt="explorer.gif">
</details>

<details>
<summary>Uploading images from input box</summary>
<img src="https://i.loli.net/2019/04/09/5cac17fe52a86.gif" alt="input box.gif">
</details>

<details>
<summary>Use selection text as the uploaded <code>fileName</code></summary>
<img src="https://i.loli.net/2019/04/09/5cac180fb1dc7.gif" alt="selection.gif">
<b>Notice: These characters: <code>\$</code>, <code>:</code>, <code>/</code>, <code>?</code> and newline will be ignored in the image name. </b>(Because they are invalid for file names.)
</details>

## Keyboard shortcuts

**You can change all the shortcuts below as you wish.**

| OS           | Uploading an image from clipboard               | Uploading images from explorer                  | Uploading an image from input box               |
| ------------ | ----------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- |
| Windows/Unix | <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>U</kbd> | <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>E</kbd> | <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>O</kbd> |
| OsX          | <kbd>Cmd</kbd> + <kbd>Opt</kbd> + <kbd>U</kbd>  | <kbd>Cmd</kbd> + <kbd>Opt</kbd> + <kbd>E</kbd>  | <kbd>Cmd</kbd> + <kbd>Opt</kbd> + <kbd>O</kbd>  |

## Settings

- Default
  - The default image hosting is [SM.MS](https://sm.ms/).

- Custom

    <details>
    <summary><b>We can customize the settings in VSCode settings</b></summary>
    <img src="https://i.loli.net/2019/04/09/5cac1821b6621.png" alt="vscode-setting.png">
    </details>

  - Use an external configuration file

    <details>
    <summary>Enter the path of the configuration file</summary>
    <img src="https://i.loli.net/2019/04/09/5cac1836598a8.png" alt="external-config.png">
    </details>

  - Use VSCode settings

    <details>
    <summary>First, choose the current PicBed</summary>
    <img src="https://i.loli.net/2019/04/09/5cac1847b5907.png" alt="current-picbed.png">
    </details>

    <details>
    <summary>Then, input all the info the current PicBed needs</summary>
    <img src="https://i.loli.net/2019/04/09/5cac4950d176b.png" alt="picbed-info.png">
    </details>

    <details>
    <summary>Customize the name of the image to be uploaded</summary>
    <b>Notice: If you selected some text before uploading, the selection will become the <code>fileName</code> of the image to be uploaded.</b>
    <img src="https://i.loli.net/2019/04/09/5cac189446749.png" alt="image-name.png">
    </details>

    <details>
    <summary>Customize the output format of the uploaded image</summary>
    <img src="https://i.loli.net/2019/04/09/5cac18a5c9def.png" alt="output-format.png">
    </details>

    <details>
    <summary>
       Suggested settings for  <a href='https://github.com/Molunerfinn/PicGo'>PicGo-electron</a> users (See <a href='https://picgo.github.io/PicGo-Doc/zh/guide/config.html#%E9%85%8D%E7%BD%AE%E6%89%8B%E5%86%8C'> PicGo configuration path</a> for more information):
    </summary>
    </details>

    **Notice: `YOUR_HOME_DIR` should be replaced by the path of your current user path.**

    ```json
    // Windows
    {
        "picgo.configPath":"YOUR_HOME_DIR\\AppData\\Roaming\\PicGo\\data.json",
        "picgo.dataPath": "YOUR_HOME_DIR\\AppData\\Roaming\\PicGo\\data.json"
    }

    // macOS
    {
        "picgo.configPath": "YOUR_HOME_DIR/Library/Application Support/picgo/data.json",
        "picgo.dataPath": "YOUR_HOME_DIR/Library/Application Support/picgo/data.json"
    }

    // Linux
    {
        "picgo.configPath": "YOUR_HOME_DIR/.config/picgo/data.json",
        "picgo.dataPath": "YOUR_HOME_DIR/.config/picgo/data.json"
    }
    ```



## Thanks

- [PicGo-Core](https://github.com/PicGo/PicGo-Core)
- [vs-picgo](https://github.com/PicGo/vs-picgo)

**Enjoy!**
