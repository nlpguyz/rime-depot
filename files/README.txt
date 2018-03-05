Upload IME schemata here
请在此目录中上传RIME输入法文件

每个输入法至少包含三个文件
- schema (中州韵输入方案定义文件）
- dict（中州韵输入方案字典）
- imdf（输入法描述文件，用于支持网络安装）

IMDF格式如下（以 pinyin_simp 为例）

{
  "id": "pinyin_simp",
  "name": {
    "en": "Mini pinyin (Simp)",
    "zh_CN": "袖珍简化字拼音",
    "zh_TW": "袖珍簡化字拼音",
    "default": "Mini pinyin (Simp)"
  },
  "version" : "1.0",
  "files" : [
    "pinyin_simp.schema.yaml",
    "pinyin_simp.dict.yaml"
  ]
}
