<p align="left">
    <a href="README.md">
        中文
    </a>
    <span> • </span>
    <span>
        <b>English</b>
    </span>
    <span> • </span>
    <a href="README_ja.md">
        日本語
    </a>
</p>

<p align="center">
  <a href="https://github.com/hiroi-sora/Umi-OCR">
    <img width="200" height="128" src="https://tupian.li/images/2022/10/27/icon---256.png" alt="Umi-OCR">
  </a>
</p>

<h1 align="center">Umi-OCR</h1>

<p align="center">
  <a href="https://github.com/hiroi-sora/Umi-OCR/releases/latest">
    <img src="https://img.shields.io/github/v/release/hiroi-sora/Umi-OCR?style=flat-square" alt="Umi-OCR">
  </a>
  <a href="https://github.com/hiroi-sora/Umi-OCR/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/hiroi-sora/Umi-OCR?style=flat-square" alt="LICENSE">
  </a>
  <a href="#download-releases">
    <img src="https://img.shields.io/github/downloads/hiroi-sora/Umi-OCR/total?style=flat-square" alt="forks">
  </a>
  <a href="https://star-history.com/#hiroi-sora/Umi-OCR">
    <img src="https://img.shields.io/github/stars/hiroi-sora/Umi-OCR?style=flat-square" alt="stars">
  </a>
  <a href="https://github.com/hiroi-sora/Umi-OCR/forks">
    <img src="https://img.shields.io/github/forks/hiroi-sora/Umi-OCR?style=flat-square" alt="forks">
  </a>
  <a href="https://hosted.weblate.org/engage/umi-ocr/">
    <img src="https://hosted.weblate.org/widget/umi-ocr/svg-badge.svg" alt="翻译状态">
  </a>
</p>

<div align="center">
  <h3>
    <a href="#usage">
      Usage
    </a>
    <span> • </span>
    <a href="#download-releases">
      Download Releases
    </a>
    <span> • </span>
    <a href="CHANGE_LOG.md">
      Changelog
    </a>
    <span> • </span>
    <a href="https://github.com/hiroi-sora/Umi-OCR/issues">
      Issue a problem
    </a>
  </h3>
</div>
<br>

<div align="center">
  <strong>Free, Open-source, Batch Offline OCR Software</strong><br>
  <sub>Compatible with Windows7 x64 and above</sub>
</div><br>

- **Free**: All the code of this project is open-source and completely free.
- **Convenient**: Unzip and use, run offline, no need for network.
- **Efficient**: Comes with a highly efficient offline OCR engine. As long as the computer performance is sufficient, it can be faster than online OCR services.
- **Flexible**: Supports customizable interface, and supports multiple calling methods such as command-line and HTTP API.

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ec301b55.png" alt="1-标题-1.png" style="width: 80%;"></p>

![1-标题-2.png](https://tupian.li/images/2023/11/19/6559909fdeeba.png)

## Using the Source Code:

Developers should read [Building the Project](#Build-the-Project) before proceeding.

## Download Releases:

- **GitHub** https://github.com/hiroi-sora/Umi-OCR/releases/latest
- **Source Forge** https://sourceforge.net/projects/umi-ocr
- **Lanzou** https://hiroi-sora.lanzoul.com/s/umi-ocr

<details>
<summary><b>•&nbsp;&nbsp;Scoop Installer</b> (Click to expand)</summary>

[Scoop](https://scoop.sh/) is a command-line installer for Windows that facilitates the management of multiple applications. You can install Scoop first and then use the following commands to install `Umi-OCR`:

- Add the `extras` bucket:
```
scoop bucket add extras
```

- (Optional 1) Install Umi-OCR (comes with the `Rapid-OCR` engine, better compatibility):
```
scoop install extras/umi-ocr
```

- (Optional 2) Install Umi-OCR (comes with the `Paddle-OCR` engine, slightly faster):
```
scoop install extras/umi-ocr-paddle
```

- Do not install both, as the shortcuts may be overwritten. However, you can import additional [plugins](https://github.com/hiroi-sora/Umi-OCR_plugins) to switch between different OCR engines at any time.

</details>

## Getting Started

The software release package is available in `.7z` compressed format or as a self-extracting `.7z.exe` package. The self-extracting package can be used to extract files on a computer without compression software installed.

This software does not require installation. After extraction, simply click on `Umi-OCR.exe` to start the program.

If you encounter any problems, please submit an [Issue](https://github.com/hiroi-sora/Umi-OCR/issues) and I will do my best to assist you.

## Interface Language

Umi-OCR supports multiple languages for its interface. When you open the software for the first time, it will automatically switch to the language based on your computer's system settings.

If you need to manually switch languages, please refer to the following figure, `全局设置`→`语言/Language` .

<p align="center"><img src="https://tupian.li/images/2023/11/19/65599c3f9e600.png" alt="1-标题-1.png" style="width: 80%;"></p>

## Tabbed Interface

Umi-OCR v2 is composed of a series of flexible and easy-to-use **tabbed interfaces**. You can open the required tabbed interface according to your preferences.

The top left corner of the tab bar can be used to switch **window always on top**. The top right corner can be used to **lock the tabbed interface** to prevent accidental closure during daily use.

### Screenshot OCR

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ecb4dfb4.png" alt="2-截图-1.png" style="width: 80%;"></p>

**Screenshot OCR**: After opening this page, you can use a keyboard shortcut to capture a screenshot and recognize the text in the image.

- The left-side image preview panel allows you to select and copy text with your mouse.
- The right-side recognition record panel allows you to edit text and select and copy multiple records.
- It also supports copying images from elsewhere and pasting them into Umi-OCR for recognition.

#### Paragraph Merge

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ecc62ac9.png" alt="2-截图-2.png" style="width: 80%;"></p>

About **OCR Text Post-Processing - Paragraph Merge**: This feature can organize the layout and order of OCR results to make the text more suitable for reading and use. The preset schemes are:

- **Single line**: Merge text on the same line, suitable for most scenarios.
- **Multiple lines - natural paragraphs**: Intelligently recognize and merge text belonging to the same paragraph, suitable for most scenarios, as shown in the figure above.
- **Multiple lines - code block**: Try to restore the original indentation and spacing of the text. Suitable for recognizing code snippets or scenes that require retaining spaces.
- **Vertical layout**: Suitable for vertical layout. Needs to be used in conjunction with a model library that also supports vertical layout recognition.

---

### Batch OCR

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ecdc5197.png" alt="3-批量-1.png" style="width: 80%;"></p>

**Batch OCR**: This page supports batch importing local images for recognition.

- The recognized content can be saved in various formats such as txt/jsonl/md/csv(Excel).
- Supports `text post-processing` technology, which can recognize text belonging to the same natural paragraph and merge it. It also supports multiple processing schemes such as code blocks and vertical text.
- There is no limit on the number of images that can be imported for processing at one time, and the software can automatically shut down or sleep after completing the task.

#### Ignore Regions

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ecbc0021.png" alt="3-批量-2.png" style="width: 80%;"></p>

About **OCR Text Post-Processing - Ignore Regions**: This is a special function in batch OCR that is used to exclude unwanted text in images.

- The ignore region editor can be accessed in the right column of the batch recognition page settings.
- As shown in the example above, there are multiple watermarks/LOGOs at the top and bottom right corner of the image. If these images are recognized in batches, the watermarks will interfere with the recognition results.
- Hold down the right mouse button to draw multiple rectangular boxes. The text inside these areas will be ignored during the task.
- Please try to draw the rectangular boxes larger, completely wrapping all possible positions of the watermark.

---

### Batch Documents OCR

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ecc8bfd4.png" alt="" style="width: 80%;"></p>

---

### QR Code

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ed01f5b2.png" alt="4-二维码-1.png" style="width: 80%;"></p>

**Scan Code**:

- You can capture screenshots, paste, or drag local images to read QR codes and barcodes.
- Supports multiple codes in one image.
- Supports 19 protocols, as follows:

`Aztec`,`Codabar`,`Code128`,`Code39`,`Code93`,`DataBar`,`DataBarExpanded`,`DataMatrix`,`EAN13`,`EAN8`,`ITF`,`LinearCodes`,`MatrixCodes`,`MaxiCode`,`MicroQRCode`,`PDF417`,`QRCode`,`UPCA`,`UPCE`,

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ed001437.png" alt="4-二维码-2.png" style="width: 80%;"></p>

**Generate Code**:

- Enter text to generate a QR code image.
- Supports 19 protocols and parameters such as **error correction level**.

---

### Global Settings

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ed16f4e0.png" alt="5-全局设置-1.png" style="width: 80%;"></p>

**Global Settings**: Here you can adjust the global parameters of the software. Common features include:

- One-click to add shortcuts or set auto-startup.
- Change the interface **language**. Umi supports traditional Chinese, English, Japanese, and other languages.
- Switch interface **themes**. Umi has multiple light/dark themes.
- Adjust the **font size** and **font** of the interface text.
- Switch OCR plugins.
- **Renderer**: The software interface defaults to support GPU-accelerated rendering. If you encounter screen flickering or UI misalignment on your machine, please adjust `Interface and Appearance` → `Renderer`, try switching to different rendering schemes, or turn off hardware acceleration.

---

## API Usage:

- [Command-line manual](docs/README_CLI.md)
- [HTTP API manual](docs/http/README.md)

## About Project Structure

### Repositories:

- [Main Repository](https://github.com/hiroi-sora/Umi-OCR) 👈
- [Plugin Repository](https://github.com/hiroi-sora/Umi-OCR_plugins)
- [Windows Runtime Library](https://github.com/hiroi-sora/Umi-OCR_runtime_windows)
- [Linux Runtime Library](https://github.com/hiroi-sora/Umi-OCR_runtime_linux)

## Build the Project

- [Windows](https://github.com/hiroi-sora/Umi-OCR_runtime_windows)
- [Linux](https://github.com/hiroi-sora/Umi-OCR_runtime_linux)

---

## Software Localization:

This project uses the Weblate platform for collaborative localization of the UI interface. We welcome translators to participate in the translation work. Please visit [Weblate: Umi-OCR](https://hosted.weblate.org/engage/umi-ocr/) to proofread and supplement existing languages, or add new languages online.

We extend our gratitude to the following translators for contributing to the localization of Umi-OCR:

| Translator                                                                           | Contributed Languages     |
| ------------------------------------------------------------------------------------ | ------------------------- |
| [bob](https://hosted.weblate.org/user/q021)                                          | English, 繁體中文, 日本語 |
| [Qingzheng Gao](https://github.com/QZGao)                                            | English, 繁體中文         |
| [Weng, Chia-Ling](https://hosted.weblate.org/user/ChiaLingWeng)                      | English, 繁體中文         |
| [linzow](https://hosted.weblate.org/user/linzow)                                     | English, 繁體中文         |
| [Marcos i](https://hosted.weblate.org/user/ultramarkorj9)                            | English, Português        |
| [Eric Guo](https://hosted.weblate.org/user/qwedc001)                                 | English                   |
| [steven0081](https://hosted.weblate.org/user/steven0081)                             | English                   |
| [Brandon Cagle](https://hosted.weblate.org/user/random4t4x14)                        | English                   |
| [plum7x](https://hosted.weblate.org/user/plum7x)                                     | 繁體中文                  |
| [hugoalh](https://hosted.weblate.org/user/hugoalh)                                   | 繁體中文                  |
| [Anarkiisto](https://hosted.weblate.org/user/Anarkiisto)                             | 繁體中文                  |
| [ドコモ光](https://hosted.weblate.org/user/umren190402)                              | 日本語                    |
| [杨鹏](https://hosted.weblate.org/user/ypf)                                          | Português                 |
| [Вячеслав Анатольевич Малышев](https://hosted.weblate.org/user/1969)                 | Русский                   |
| [Muhammadyusuf Kurbonov](https://hosted.weblate.org/user/muhammadyusuf.kurbonov2002) | Русский                   |
| [தமிழ்நேரம்](https://hosted.weblate.org/user/TamilNeram/)                                | தமிழ்                       |

If you find any errors in the information or missing contributors, please reply in [this discussion](https://github.com/hiroi-sora/Umi-OCR/discussions/449).

---

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=hiroi-sora/Umi-OCR&type=Date)](https://star-history.com/#hiroi-sora/Umi-OCR&Date)

## [CHANGE LOG](CHANGE_LOG.md)