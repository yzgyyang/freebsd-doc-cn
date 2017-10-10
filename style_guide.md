# 风格指南 Style Guide

## [Livid 中文 Web 阅读体验](https://web.archive.org/web/20120513134359/http://www.livid.cn/doc_view.php?doc_id=5332)

- 中文正文及标题中出现的标点符号应该使用全角方式输入。
- 中文正文及标题中出现的英文及数字应该使用半角方式输入，并且在左右各留一个半角空格。如果这些这些半角英文及数字的左边或者右边紧接着任何的中文全角括号或者其他标点符号的话，则不需要加入半角空格。
- 中文全角空格应该只在标题处使用。
- 中文的段落与段落之间应该留出一个完整的空行。

## [翻译词汇对照表](https://web.archive.org/web/20110707050306/http://www.freebsd.org.cn/cndocs/words.html)

### 前言

语言是文化的直接体现，我们要求每一位翻译小组的成员谨记。在翻译过程中，对于所有的术语和语法，我们强制性要求使用中国大陆的习惯和标准。以下术语表将起到一个规范术语的作用，请参加翻译的朋友务必遵守。

### 保持英文原文的建议

- 众所周知的术语（对照表中将给出建议）
- 英文人名
- 系统显示的信息
- 系统命令
- 系统调用或函数
- 系统账号或用户
- 系统文件或目录名称

### 翻译词汇对照表

| 英语原文 | 中文翻译 | 备注 |
|-|-|-|
| administrator | 管理员 | 特指 Windows 系统管理员账号“Administrator”请保持英语原文 |
| advanced | 先进（的），高级（的）||
| boot | 引导 ||
| Boot Manager | 引导管理器 ||
| CD / CD-ROM / CDROM | 光盘 ||
| CD / CD-ROM / CDROM driver | 光盘驱动器，光驱 ||
| configure | 配置，设置 ||
| configuration | 配置，设置 | 也可指配置文件，根据上下文理解 |
| copy | 名词：副本；动词：复制 | 请勿音译为“拷贝” |
| delete | 删除 ||
| detect | 检测 ||
| device | 设备 ||
| disk | 磁盘 ||
| driver | 驱动器，驱动程序 ||
| edit | 编辑 ||
| editor | 编辑器，编辑（职务）||
| edition | 版，版次，版本 ||
| Email / E-mail | 电子邮件 | 也可保持英文原文，请勿翻译为“电子函件” |
| file | 文件 ||
| floppy disk | 软盘 ||
| floppy disk driver | 软盘驱动器，软驱 ||
| forced | 强制（的）||
| get | 获取 ||
| hard disk | 硬盘 ||
| hardware | 硬件 ||
| information | 信息 ||
| install | 安装 ||
| Internet | 互联网 | 也可保持英文原文，请勿翻译为“因特网” |
| load | n. 负荷，负载；v. 加载 ||
| mail | 邮件 ||
| message | 信息，消息 | 有时可译作“邮件” |
| mode | 模式 ||
| net | 网 ||
| network | 网络 ||
| open | 打开，开启 ||
| Operating System (OS) | 操作系统 ||
| remove | 删除（文件），移除、取出、拿掉（物理设备）||
| root | 根 | 特指 UNIX 系统管理员账号“root”请保持英语原文 ||
| setup | 安装，配置 ||
| software | 软件 ||
| window | 窗口 ||
| Windows || 特指微软操作系统“Windows”请保持英语原文 |
| X Window || 特指 UNIX 桌面环境“X Window”请保持英语原文 |

## [Tips for Translators](https://www.freebsd.org/doc/en_US.ISO8859-1/books/fdp-primer/po-translations-tips.html)

### 12.5.1. Preserving XML Tags
Preserve XML tags that are shown in the English original.

Example: Preserving XML Tags
English original:
```
If <acronym>NTP</acronym> is not being used
```
Spanish translation:
```
Si <acronym>NTP</acronym> no se utiliza
```

### 12.5.2. Preserving Spaces
Preserve existing spaces at the beginning and end of strings to be translated. The translated version must have these spaces also.

### 12.5.3. Verbatim Tags
The contents of some tags should be copied verbatim, not translated:

```
<citerefentry>
<command>
<filename>
<literal>
<manvolnum>
<orgname>
<package>
<programlisting>
<prompt>
<refentrytitle>
<screen>
<userinput>
<varname>
```

### 12.5.4. $FreeBSD$ Strings
The $FreeBSD$ version strings used in files require special handling. In examples like Example 12.1, “Creating a Spanish Translation of the Porter's Handbook”, these strings are not meant to be expanded. The English documents use `&dollar;` entities to avoid including actual literal dollar signs in the file:
```
&dollar;FreeBSD&dollar;
```
The &dollar; entities are not seen as dollar signs by the version control system and so the string is not expanded into a version string.

When a PO file is created, the &dollar; entities used in examples are replaced with actual dollar signs. The resulting literal $FreeBSD$ string will be wrongly expanded by the version control system when the file is committed.

The same technique as used in the English documents can be used in the translation. The &dollar; is used to replace the dollar sign in the translation entered into the PO editor:
```
&dollar;FreeBSD&dollar;
```
