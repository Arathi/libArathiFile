#Arathi文件库(libArathiFile)功能描述

##archive 档案文件类

#### archive(string $name) 构造函数
初始化了5个成员属性（均为数组）：

* options 选项，包含如下：
  - basedir 基础目录，默认值"."
  - name 名称，设置为传入参数$name
  - prepend 默认值""
  - inmemory 默认值0
  - overwrite 默认值0
  - recurse 默认值1
  - storepaths 默认值1
  - followlinks 默认值0
  - level 级别，默认值3
  - method 方法，默认值1
  - sfx 默认值""
  - type 默认值""
  - comment 注释，默认值""
* files 文件列表
* exclude 
* storeonly   
* error       

#### set_options(array $options) 设置归档选项
将$options数组中的元素搬到成员options中。有三个值要特殊处理：

* basedir
* name
* prepend

#### create_archive() 创建档案文件
#### add_data($data) 添加数据？
#### make_list() 创建列表？
#### add_files($list) 添加文件
#### exclude_files($list) 排除文件
#### store_files($list) 记录文件
#### list_files($list) 列出文件列表
#### parse_dir($dirname) 粘贴目录
#### sort_files($a, $b) 排序
#### download_file() 下载文件

##tar_file tar文件类

#### tar_file(string $name) 构造函数
#### create_tar() 创建tar包
#### extract_files() 解压文件
#### open_archive() 打开档案文件

## gzip_file gz文件类

#### gzip_file(string $name) 构造函数
#### create_gzip() 创建gz包
#### open_archive() 打开档案文件

## bzip_file bz文件类

#### bzip_file(string $name) 构造函数
#### create_bzip() 创建bz包
#### open_archive() 打开档案文件

## zip_file zip文件类

#### zip_file(string $name) 构造函数
#### create_zip() 创建zip包

## AFL提供的文件管理函数

#### int ext_size(string $target) 扩散型大小获取
可以获取单个文件或者整个目录的大小

#### bool ext_delete(string $target) 扩散型删除
可以删除单个文件或者整个目录

#### bool ext_copy(string $src, string $dest) 扩散型复制
可以复制单个文件或者整个目录

#### download_to_server($string $url) 下载文件到服务器
目前还只是实现了功能而已


