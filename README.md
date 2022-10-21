# CLAN Studio Toolkits - Icon Creator

下载地址：[clan_studio_lib_cstk_icon_creator-1.0.0.1.vip](https://github.com/clan4456/CSTK_Icon_Creator/releases/download/v1.0.0.1/clan_studio_lib_cstk_icon_creator-1.0.0.1.vip)

SHA-256：3a297c5a6588154b9eca7ed7f3f5f266be6f316f26b662ca6b70933bd54aa763

## 1. 简介

![Snipaste_2022-10-20_14-57-51.png](http://pic2.clan4456.com/clan-picgo-core/images/2022/10/20/Snipaste_2022-10-20_14-57-51-d63c19ac2ca6cb12f6296461605eca9c.png!small)

本工具主要用于生成规范化图标模板，左上角为可配置的自定义标志，右上角为图标模板标题，无标志情况下支持7个字符，有标志情况下支持5个字符。标题字体可选择 Small Fonts 或 6px2bus 。 Small Fonts 为 LabVIEW 开发环境安装时自带， 6px2bus 字体安装方式详见下文。标题字体颜色、标题背景颜色、主题背景颜色均可自定义。

设置完毕后，点击“生成”按钮可预览图标，预览后再点击“保存”按钮，自动保存。图标模板保存路径为`%USERPROFILE%\Documents\LabVIEW Data\Icon Templates\CLAN Studio\`中，按自定义标志分类。

保存的图标模板一共5个，其中通用模板4个（1~4），控件模板1个（Ctl）。

![Snipaste_2022-10-20_15-08-38.png](http://pic2.clan4456.com/clan-picgo-core/images/2022/10/20/Snipaste_2022-10-20_15-08-38-4a38673d9e3fd4db3cff6ee67d3d27b4.png!small)

## 2. 前置库

本工具使用到`OpenG Array Library`和`OpenG File Library`两个OpenG库，需通过VIPM提前安装，亦可在安装本工具时自动安装。

## 3. 字体安装

下载本仓库Fonts文件夹中的`6PX2BUS_symbol.ttf`字体，并右击，选择“ ***为所有用户安装*** ”。

## 4. Small Fonts字体清晰度调整

用记事本打开LabVIEW程序安装目录下的“LabVIEW.ini”配置文件，在末尾增加以下一行，并保存。

```ini
FontCodePageList=Small Fonts,1252
```

## 5. 安装Icon Creator

下载Release中的`clan_studio_lib_cstk_icon_creator-1.0.0.1.vip`，并双击通过VIPM进行安装。（需安装VIPM 2014或以上版本）

## 6. 打开Icon Creator

安装 ***Icon Creator*** 后，可通过LabVIEW的“工具”-->“CLAN Studio Toolkits”-->“CSTK_Icon_Creator”打开。

## 7. 使用图标模板

在生成并保存图标模板后，只需打开图标编辑器，点击“模板”中的刷新按钮，即可看到刚才生成的图标模板。

![Snipaste_2022-10-20_15-27-53.png](http://pic2.clan4456.com/clan-picgo-core/images/2022/10/20/Snipaste_2022-10-20_15-27-53-a89aa47b1e9604c860199e6a932f25f3.png!small)

## 8. 自定义标志

本工具支持自定义标志，可通过以下路径（以默认安装LabVIEW 2015 x86为例，其他版本则对应修改路径）进行自定义标志增加。

```shell
C:\Program Files (x86)\National Instruments\LabVIEW 2015\vi.lib\CLAN Studio\CLAN Studio Toolkits - Icon Creator\Library\Icon Creator\Template
```

为每个自定义标志建立一个文件夹（其中Default文件夹为无标志模板，不能删除），文件夹里面放置5个png格式的图标模板，文件名称需保持不变。可以“CLAN”文件夹为参考，修改每个模板的左上角标志位置样式即可。

## 9. 已知bug

暂未发现

## 10. 开源许可

本工具遵循BSD开源协议，可任意分发或二次开发使用。但需保留UI界面上的CLAN Studio标志即可。
