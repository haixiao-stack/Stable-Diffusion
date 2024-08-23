# Stable-Diffusion

## Controlnet实战

​	利用Controlnet中的OpenPose人物绘制的姿势控制，使得生成图片与原图姿态动作相似，Lineart线稿上色，使得生成图片与线稿图片的人物保持一致，Tile模块结合Tile VAE以及Tile Diffusion实现图片高清放大，使得重绘幅度较大的时候能够保持原图细节

### OpenPose



<center>
<figure>
    <img src=".\pictures\openpose-1.png" align="center" width=256 height=256>
    <img src=".\pictures\openpose-2.png" align="center" width=512 height=256>
</figure>
</center>

​		            **原图** 											**Contronet对比图** 

### Lineart

<center>
<figure>
    <img src=".\pictures\lineart-1.png" align="center" width=256 height=256>
    <img src=".\pictures\lineart-2.png" align="center" width=512 height=256>
</figure>
</center>

​		            **原图** 											**Contronet对比图** 

### Tile

<center>
<figure>
    <img src=".\pictures\tile-1.png" align="center" width=256 height=256>
    <img src=".\pictures\tile-2.png" align="center" width=512 height=256>
</figure>
</center>

​		            **原图** 											**Contronet对比图** 



## Lora微调

​	选取15张中国古风花鸟画图片，利用Dataset Tag Editor进行标签生成并将guofeng作为触发词放置在每个标签前面，并将图像裁剪成768*512做成训练集，以liblib.AI网站上的古风绘画写实向模型为checkpoint模型进行Lora微调模型的训练，训练后给定提示词生成具有中国古风的花鸟图

<center>
<figure>
    <img src=".\pictures\lora-1.png" align="center" width=1028 height=512>
</figure>
</center>	

<center>
<figure>
    <img src=".\pictures\lora-2.png" align="center" width=1028 height=512>
</figure>
</center>	