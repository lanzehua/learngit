# 10.8工作小结：

---

1. Paper：Generative Adversarial Text to Image Synthesis

![image-20221008113252095](C:\Users\lzhrt\AppData\Roaming\Typora\typora-user-images\image-20221008113252095.png)

![在这里插入图片描述](https://img-blog.csdnimg.cn/20191023152502634.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L05HVWV2ZXIxNQ==,size_16,color_FFFFFF,t_70)

![image-20221008133226368](C:\Users\lzhrt\AppData\Roaming\Typora\typora-user-images\image-20221008133226368.png)

![image-20221008135714903](C:\Users\lzhrt\AppData\Roaming\Typora\typora-user-images\image-20221008135714903.png)

文本被经过一个全连接后连接到noise上输入G中进行运算

![image-20221008140822050](C:\Users\lzhrt\AppData\Roaming\Typora\typora-user-images\image-20221008140822050.png)

![image-20221008140957316](C:\Users\lzhrt\AppData\Roaming\Typora\typora-user-images\image-20221008140957316.png)

在本文中，图像分类器用的是GoogLeNet，文本分类器用的是LSTM和CNN。

得到文本特征后，需要把文本特征压缩后与图像特征拼接在一起，放入DC-GAN。

随后本文还提出了一个差值学习**4.3. Learning with manifold interpolation (GAN-INT)**

![image-20221008143539792](C:\Users\lzhrt\AppData\Roaming\Typora\typora-user-images\image-20221008143539792.png)

![image-20221008143752347](C:\Users\lzhrt\AppData\Roaming\Typora\typora-user-images\image-20221008143752347.png)

![image-20221008143840654](C:\Users\lzhrt\AppData\Roaming\Typora\typora-user-images\image-20221008143840654.png)

插值法的妙用\Uparrow$

![image-20221008144421337](C:\Users\lzhrt\AppData\Roaming\Typora\typora-user-images\image-20221008144421337.png)

随后翻转G进行风格迁移



tips： zero-shot learning 零样本学习![img](https://img-blog.csdnimg.cn/b2c6c8c6a33e48a0bd1ef8ce76dfacd4.png)

![image-20221008151346142](C:\Users\lzhrt\AppData\Roaming\Typora\typora-user-images\image-20221008151346142.png)

为了量化对幼崽的解缠程度，我们设置了两个以噪声z作为输入的预测任务：姿态鉴别和色彩鉴别





2. 学习了sftp和xftp的使用
3. 配置了服务器一个