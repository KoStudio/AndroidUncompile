#### Apk反编译过程：

1.  `.apk →.zip`,  打开找到`classes.dex`文件(Dalvik VM的所有类都在这里)
  
2.  用`dex2jar-0.0.9.12`里的`dex2jar.sh` (windows 用`dex2jar.bat`)进行反编译,会在`dex2jar`的目录上生成`classes_dex2jar.jar`文件 
  > 拷贝 `classes.dex`文件到`dex2jar.sh`相同目录下:
  > 输入命令： `dex2jar.sh classes.dex`

3. 用`JD-GUI`查看`jar`文件

4. 用`AXMLPrinter2.jar`反编译`XML`文件
  > 命令格式：`java -jar AXMLPrinter2.jar D:\play\AndroidManifest.xml > AndroidManifest.txt`