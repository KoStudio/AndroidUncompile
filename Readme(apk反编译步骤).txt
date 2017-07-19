Apk反编译过程：

1.  .apk →.zip,打开找到classes.dex文件(Dalvik VM的所有类都在这里)
2.  用dex2jar-0.0.9.12里的dex2jar.sh (windows 用dex2jar.bat)进行反编译会在dex2jar的目录上生成classes_dex2jar.jar文件 (copy classes.dex文件到dex2jar.sh相同目录下)
3.用JD-GUI查看jar文件
4.用AXMLPrinter2.jar反编译XML文件
  命令格式：java -jar AXMLPrinter2.jar D:\play\AndroidManifest.xml > AndroidManifest.txt

（http://www.cnblogs.com/stulife/archive/2010/08/24/1807143.html）