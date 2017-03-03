# imagesUtils
you can use it to load images
图片处理的一个工具类，可以对图片进行压缩


**Android OOM** 在Android中加载图片，很容易出现OOM，尤其是在加载大图或者加载很多图片的时候，这个时候我们要对图片进行一定的压缩处理，在不影响用户体验的情况下降低图片的质量，比如使用GRB_565.在图片操作处理完后最好手动释放资源。
> **注意：从3.0开始，Bitmap像素数据和Bitmap对象一起存放在Dalvik堆中，而在3.0之前，Bitmap像素数据存放在Native内存中。所以，在3.0之前，Bitmap像素数据在Nativie内存的释放是不确定的，容易内存溢出而Crash，官方强烈建议调用recycle()（当然是在确定不需要的时候）；而在3.0之后，则无此要求。


 ----------------------------------------------------------------------------------------------------------------------------
 #下面主要测试MarkDown的使用
- **功能丰富** ：支持高亮代码块、*LaTeX* 公式、流程图，本地图片以及附件上传，甚至截图粘贴，工作学习好帮手；
- **得心应手** ：简洁高效的编辑器，提供[桌面客户端][1]以及[离线Chrome App][2]，支持移动端 Web；
- **深度整合** ：支持选择笔记本和添加标签，支持从印象笔记跳转编辑，轻松管理。

### 代码块
``` java
public class BitmapFactory {
    public static class Options {
        public boolean inScaled;     // 默认true
        public int inDensity;        // 无dpi的文件夹下默认160
        public int inTargetDensity;  // 取决具体屏幕
    }
}
```

### 表格
| Item      |    Value | Qty  |
| :-------- | --------:| :--: |
| Computer  | 1600 USD |  5   |
| Phone     |   12 USD |  12  |
| Pipe      |    1 USD | 234  |
