#Arathi文件库(libArathiFile)功能描述

##archive 档案文件类

### archive($name) 构造函数
### set_options($options) 设置归档选项
### create_archive() 创建档案文件
### add_data($data) 添加数据？
### make_list() 创建列表？
### add_files($list) 添加文件
### exclude_files($list) 排除文件
### store_files($list) 记录文件
### list_files($list) 列出文件列表
### parse_dir($dirname) 粘贴目录
### sort_files($a, $b) 排序
### download_file() 下载文件

##tar_file tar文件类

### tar_file($name) 构造函数
### create_tar() 创建tar包
### extract_files() 解压文件
### open_archive() 打开档案文件

## gzip_file gz文件类

### gzip_file($name) 构造函数
### create_gzip() 创建gz包
### open_archive() 打开档案文件

## bzip_file bz文件类

### bzip_file($name) 构造函数
### create_bzip() 创建bz包
### open_archive() 打开档案文件

## zip_file zip文件类

### zip_file($name) 构造函数
### create_zip() 创建zip包

## AFL提供的文件管理函数

### ext_size($target) 扩散型大小获取
可以获取单个文件或者整个目录的大小

### ext_delete($target) 扩散型删除
可以删除单个文件或者整个目录

### ext_copy($target) 扩散型复制
可以复制单个文件或者整个目录

















