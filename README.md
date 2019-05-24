shumei.py为主文件，直接运行即可  
  
加解密方式 des mode：ECB padding：ZEROPADDING  
代码中的轨迹是按照 math.sin 生成  
缺口距离使用 cv2.matchTemplate 方法，有几率识别错误  
  
1.从接口中获得k、图片、rid  
2.将k解密，生成用于加密轨迹等参数的key，解密key为 sshummei  
3.参数主要包括m:轨迹  等等，都有注释  
4.用加密 k 后的值取八个字符当做新 key 加密参数  
