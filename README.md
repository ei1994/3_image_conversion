## 3、image_conversion
基于图像转换的异源图像块匹配方法

## train_nature_X.py：训练和测试的代码；model_d_X：模型的代码

train_gd_gray2nir.py：GAN网络，用于将可见光图像转换为近红外图像
train_nature_map_gd.py：训练及测试代码

train_gd_nir2nir.py: 自编码器，用于近红外图像的特征提取
train_gd_gray2nir_pro.py：GAN网络，加入了自编码器的编码器进行约束
train_nature_map_gd_pro.py：训练及测试代码

## 简介
基于图像转换的异源图像块匹配方法。针对异源图像之间存在的表征差异性问题，利用生成对抗网络中的生成器将异源图像转换为同源图像，之后对同源图像进行相似性度量，以此降低匹配难度。为改善生成的转换图像质量及多样性，通过预训练的卷积自编码器来正则约束判别器网络的训练，从而间接强化生成器的稳定训练。图像转换策略克服了图像之间由于表征差异性大导致的匹配困难问题，为异源图像匹配提供了全新的解决思路。

Third, heterogeneous image patches matching method based on image conversion. Aiming at the problem of characterization differences between heterogeneous images, the generator in GAN is used to convert the heterogeneous images into the homologous images, and then similarity measures are performed on homologous images to reduce the difficulty of matching. In order to improve the quality and diversity of the generated images, the pre-trained convolution auto-encoder is used to regularly constrain the training of the discriminator network in GAN, thereby indirectly enhancing the stable training of the generator. The strategy of image conversion overcomes the difficulty of matching between images due to the considerable characterization differences and provides a new solution for heterogeneous image matching.
