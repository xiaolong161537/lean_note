# lean_note
该仓库用来记录一些开发中遇到的问题

2020/4/30 sqlyog修改utf8字符集校对时无法修改，导致连表查询报错， 解决：使用sql语句修改
校对主要用于字段排序
utf8_unicode_ci和utf8_general_ci对中、英文来说没有实质的差别。
utf8_general_ci 校对速度快，但准确度稍差。
utf8_unicode_ci 准确度高，但校对速度稍慢。
若数据库中有德语、法语或者俄语需求，需使用utf8_unicode_ci。
其他情况用utf8_general_ci即可。
