# 项目管理笔记
//批量重命名以zheng开头的文件，	改为以ebey开头的文件
for file in `find . -name 'zheng*' -exec basename {} \;`; do mv $file ${file/zheng/ebey};done


//不递归
find . -maxdepth 1 -name 'zheng*'


//直到没有 类似 “No such file or directory” 报错为止~
for file in `find . -name 'zheng*' `; do mv $file ${file/zheng/ebey};done