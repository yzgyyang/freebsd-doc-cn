# 风格指南 Style Guide

## [Livid 中文 Web 阅读体验](https://web.archive.org/web/20120513134359/http://www.livid.cn/doc_view.php?doc_id=5332)

- 中文正文及标题中出现的标点符号应该使用全角方式输入。
- 中文正文及标题中出现的英文及数字应该使用半角方式输入，并且在左右各留一个半角空格。如果这些这些半角英文及数字的左边或者右边紧接着任何的中文全角括号或者其他标点符号的话，则不需要加入半角空格。
- 中文全角空格应该只在标题处使用。
- 中文的段落与段落之间应该留出一个完整的空行。

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
