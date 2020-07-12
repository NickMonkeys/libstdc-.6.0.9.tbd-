# 用于解决xcode异常

## 异常特征：
library not found -lstdc++.6.0.9

## 异常日志：
```
ld: library not found for -lstdc++.6.0.9
clang: error: linker command failed with exit code 1 (use -v to see invocation)
```

## 异常说明：
这是因为xcode中引用了libstdc++.6.0.9.tbd这个文件，而Xcode10移除了这个文件。  
我们可以去Xcode9中移出该文件，路径为：  
/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/SDKs/iPhoneOS.sdk/usr/lib/


[CSDN](https://mp.csdn.net/console/editor/html/103680831)
