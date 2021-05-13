### Windows下使用cmake编译C项目

1. 安装MinGW

2. 找到MinGW安装目录，将mingw32-make.exe重命名为make.exe

3. 在写好的c项目工程中执行make.命令
   可能会遇到没有MakeFiles文件的情况，解决方案：

   ```
   删除目录下的CMakeCache.txt(如果有的话)
   执行cmake . -G "Unix MakeFiles";
   然后就生成MakeFIles文件了
   ```

4. 执行make即可生成可执行文件

