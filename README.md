# DoNotDeleteMyFile
DoNotDeleteMyFile-规避网盘文件和谐
 
 本软件可以实现在任何类型的文件末尾添加一串随机生成的Key, 籍此来改变文件的md5,CRC等特征值, 并且不影响文件主要内容.
 以及在文件开头加入一串随机生成的Key, 阻止审查者直接读取文件,同时改变文件的md5,CRC等特征值, 主要适用于视频, word等. 
 由此来达到规避网盘文件审查的目的.
 
 经过测试不会对pdf,视频,压缩包等文件产生影响, 即便产生影响, 也可以用软件一键删除之前添加的key.
 
 # 使用说明
 
 AddKey.py负责向文件末尾添加key, key由软件自己随机生成, 输入文件所在路径+文件名后按回车即可, 处理成功后提示'Success!!',被加入key的文件将保存在'KeyAdded'文件夹内.(该文件夹和脚本在同一文件夹内)
 
 Delkey.py负责删除之前添加的Key(AddKey和FakeEncrypt的key均可以), 同样输入文件所在路径+文件名后按回车即可, 处理成功后提示'Success!!',被去除key的文件将保存在'Original'文件夹内.(该文件夹和脚本在同一文件夹内)
 
 新增的FakeEncrypt.py在文件开头加入一串随机生成的Key, 阻止审查者直接读取文件, 对简单的批量审查较为有效, 审查者会认为这是一个损坏的无效文件放弃审查, 同时也可以改变文件的md5,CRC等特征值, 主要适用于视频, word等. 使用时输入文件所在路径+文件名后按回车即可, 处理成功后提示'Success!!',被"假加密"的文件将保存在'FakeEncrypted'文件夹内.(该文件夹和脚本在同一文件夹内)
 
 运行AddKey和FakeEncrypt后会生成 FileAndKey.json , 该文件的作用是记录之前生成的key和对应的文件名, 方便以后使用Delkey来删除key, 请勿删除该文件, 如果误删, 请用 notepad++或者Windows自带记事本等软件手动打开文件, 自行删除添加的key, key的格式为:'#DoNotDelMyFile//随机数字#'
 
 # 免责声明
 
 本软件开源免费, 使用及修改造成的后果由您自己负责,与本人无关.
