# DoNotDeleteMyFile
DoNotDeleteMyFile-规避网盘文件和谐
 
 本软件可以实现在任何类型的文件末尾添加一串随机生成的Key, 籍此来改变文件的md5,CRC等特征值, 并且不影响文件主要内容.
 由此来达到规避网盘文件审查的目的.
 
 经过测试不会对pdf,视频,压缩包等文件产生影响, 即便产生影响, 也可以用软件一键删除之前添加的key.
 
 # 使用说明
 
 AddKey.py负责向文件末尾添加key, key由软件自己随机生成, 输入文件所在路径+文件名后按回车即可, 处理成功后提示'Success!!',文件修改将直接在你输入的文件上进行, 不会另外生成文件, 所以请注意数据安全.
 
 Delkey.py负责删除之前添加的Key, 同样输入文件所在路径+文件名后按回车即可, 处理成功后提示'Success!!',并且会生成一个新文件,
 即去除key以后的原文件'filename_Original.xxx'.
 
 # 免责声明
 
 本软件开源免费, 使用及修改造成的后果由您自己负责,与本人无关.
