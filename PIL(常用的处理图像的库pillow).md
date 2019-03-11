[官网](https://pillow.readthedocs.io/en/5.2.x/)  
[某个博客](https://blog.csdn.net/zhangziju/article/details/79123275)  

pip3 install pillow  
bytesIO


# open
```
    from PIL import Image             #调用库
    im = Image.open("E:\mywife.jpg")  #文件存在的路径
```
# 截图
```
from PIL import ImageGrab
im = ImageGrab.grab((0,0,100,100))  #(box)
im.save("123.png")
```
# 裁剪
```
from PIL import Image
im = Image.open("1.jpg")
im = im.crop((0,0,100,100))
im.save("233.png")
```
# 获取图像尺寸
```
from PIL import Image
im = Image.open("1.jpg")
im.size
```
# 黑白
```
from PIL import Image
im = Image.open("1.jpg")
im=im.convert("L")
im.show()
```    
# 色块遮挡特定区域

```
from PIL import Image

im = Image.open("1.jpg")
new_image= Image.new("RGBA", (128, 128), "blue")    #新建纯色图片
im.paste(new_image, (0, 0, 128, 128))   #粘贴特定区域
im.show()
```
# 获得每个像素的rgb矩阵

```
from PIL import Image

im = Image.open("1.jpg")
pixel = im.load()
print(pixel[0,0])
```
