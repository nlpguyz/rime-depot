# rime-depot
Collection of installable RIME input schemata
用于安卓黑客键盘的中州韵输入方案汇集（欢迎提交）

# Help
请在此目录中上传RIME输入方案相关文件（schema和dict等），并新建一个imdf描述文件，用于输入方案的网络安装。

在上传输入方案时，请提供至少三个文件：
- schema (中州韵输入方案主文件，如 pinyin_simp.schema.yaml）
- dict（中州韵字典，如 pinyin_simp.dict.yaml）
- imdf（新输入法描述文件，如 pinyin_simp.imdf）

网络安装输入方案需要知道一个输入方案所需要的所有文件，通常为两个文件xxxx.schema和xxxx.dict，但也可能包括其他的依赖文件，如多个字典文件，以及依赖的输入方案等。因此在贡献输入方案时，请同时提交imdf文件。除了指定所安装的文件外，imdf文件还包含多语言界面所需要的提示信息和版本等。具体格式请见下例。

IMDF格式如下（以 pinyin_simp 为例）
<pre>
{
  "id": "pinyin_simp",             // 此ID应该与schema文件中的ID相同
  "name": {
    "en": "Mini pinyin (Simp)",    // 英文名可以任意
    "zh_CN": "袖珍简化字拼音",       // 中文名可以任意，但最好与中州韵schema文件相同（改为简体）
    "zh_TW": "袖珍簡化字拼音",       // 繁体中文可以任意，但最好与中州韵schema文件相同（改为繁体）
    "default": "Mini pinyin (Simp)"  // 缺省名，建议用英文或者中文
  },
  "version" : "1.0",               // 版本可以任意，原则上最好与schema相同
  "files" : [
    "pinyin_simp.schema.yaml",
    "pinyin_simp.dict.yaml"
  ]
}
</pre>
