# JPEG restoration

## 1.传统方法

1.Howard C Reeve III and Jae S Lim. Reduction of blocking effects in image coding. Optical Engineering, 23(1):34–37, 1984.
2.Peter List, Anthony Joch, Jani Lainema, Gisle Bjontegaard, and Marta Karczewicz. Adaptive deblocking filter. IEEE Trans. Circuit Syst. Video Technol., 13(7):614–619, 2003.
3.Seok Bong Yoo, Kyuha Choi, and Jong Beom Ra. Postprocessing for blocking artifact reduction based on interblock correlation. IEEE Trans. Multimedia, 16(6):15361548, 2014.
4.Kostadin Dabov, Alessandro Foi, Vladimir Katkovnik, and Karen Egiazarian. Image denoising by sparse 3-d transform-domain collaborative filtering. IEEE Trans. Image Process., 16(8):2080–2095, 2007.

5.Alessandro Foi, Vladimir Katkovnik, and Karen Egiazarian, “Pointwise shape-adaptive dct for high-quality denoising and deblocking of grayscale and color images,” IEEE Transactions on Image Processing, vol. 16, no. 5, pp. 1395–1411, 2007.

**传统DCT域方法**

1.Alessandro Foi, Vladimir Katkovnik, and Karen Egiazarian. “Pointwise shapeadaptive DCT for high-quality deblocking of compressed color images”. In: 2006 14th European Signal Processing Conference. IEEE. 2006, pp. 1–5.

2.Seungjoon Yang et al. “Blocking artifact free inverse discrete cosine transform”. In: Proceedings 2000 International Conference on Image Processing (Cat. No. 00CH37101). Vol. 3. IEEE. 2000, pp. 869–872.

3.Xueyang Fu et al. “JPEG Artifacts Reduction via Deep Convolutional Sparse Coding”. In: Proceedings of the IEEE International Conference on Computer Vision. 2019, pp. 2501–2510.

## 2. 基于Sparse coding的方法

1.Huibin Chang, Michael K Ng, and Tieyong Zeng, “Reducing artifacts in jpeg decompression via a learned dictionary,” IEEE Transactions on Signal Processing, vol. 62, no. 3, pp. 718–728, 2014.

2.Xianming Liu, Xiaolin Wu, Jiantao Zhou, and Debin Zhao, “Data-driven sparsity-based restoration of jpeg-compressed images in dual transform-pixel domain.,” in Proceedings of the IEEE International Conference on Computer Vision and Pattern Recognition, 2015, vol. 1, p. 5.

## 3.基于深度学习的方法

### 像素域的方法

1.Kai Zhang, Wangmeng Zuo, Yunjin Chen, Deyu Meng, and Lei Zhang, “Beyond a Gaussian denoiser: Residual learning of deep CNN for image denoising,” IEEE Transactions on Image Processing, vol. 26, no. 7, pp. 3142–3155, 2017.

2.Chao Dong, Yubin Deng, Chen Change Loy, and Xiaoou Tang, “Compression artifacts reduction by a deep convolutional network,” in Proceedings of the IEEE International Conference on Computer Vision, 2015, pp. 576–584.

3.Lukas Cavigelli, Pascal Hager, and Luca Benini, “Cas-cnn: A deep convolutional neural network for image compression artifact suppression,” in Proceedings of the International Joint Conference on Neural Networks (IJCNN). IEEE, 2017, pp. 752–759.（**多尺度的loss**）

4.Ying Tai, Jian Yang, Xiaoming Liu, and Chunyan Xu, “Memnet: A persistent memory network for image restoration,” in Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition, 2017, pp. 4539–4547.

5.Jianwei Li, Yongtao Wang, Haihua Xie, and Kai-Kuang Ma. Learning a single model with a wide range of quality factors for jpeg image artifacts removal. IEEE Trans. Image Process., 29:8842–8854, 2020.

6.Xueyang Fu, Menglu Wang, Xiangyong Cao, Xinghao Ding, and Zheng-Jun Zha. A model-driven deep unfolding method for jpeg artifacts removal. IEEE Trans. Neural Netw. Learn. Syst., 33(11):6802–6816, 2022.

7.Jeonghwan Yoon and Nam Ik Cho. Jpeg artifact reduction based on deformable offset gating network controlled by a variational autoencoder. IEEE Access, 11:30282–30291, 2023.

8.Xi Wang, Xueyang Fu, Yurui Zhu, and Zheng-Jun Zha. Jpeg artifacts removal via contrastive representation learning. In Proc. Eur. Conf. Comput. Vis., Tel Aviv, Israel, pages 615–631. Springer, 2022.



**预测质量因素**

1.Jiaxi Jiang, Kai Zhang, and Radu Timofte. Towards flexible blind jpeg artifacts removal. In Proc. IEEE Int. Conf. Comput. Vis., pages 4997–5006, 2021.

2.Yoonsik Kim, Jae Woong Soh, Jaewoo Park, Byeongyong Ahn, Hyun-Seung Lee, Young-Su Moon, and Nam Ik Cho. A pseudo-blind convolutional neural network for the reduction of compression artifacts. IEEE Trans. Circuit Syst. Video Technol., 30(4):1121–1135, 2020.

3.Yoonsik Kim, Jae Woong Soh, and Nam Ik Cho. “AGARNet: Adaptively Gated JPEG Compression Artifacts Removal Network for a Wide Range Quality Factor”. In: IEEE Access 8 (2020), pp. 20160–20170.

4.Leonardo Galteri et al. “Deep universal generative adversarial compression artifact removal”. In: IEEE Transactions on Multimedia (2019).（**基于GAN**）

**每个质量因素都训练**

1.Pavel Svoboda, Michal Hradis, David Barina, and Pavel Zemcik. Compression artifacts removal using convolutional neural networks. arXiv preprint arXiv:1605.00366, 2016.
2.Chao Dong, Yubin Deng, Chen Change Loy, and Xiaoou Tang. Compression artifacts reduction by a deep convolutional network. In Int. Conf. Comput. Vis., pages 576–584, 2015.
3.Yulun Zhang, Kunpeng Li, Kai Li, Bineng Zhong, and Yun Fu. Residual non-local attention networks for image restoration. In Int. Conf. Learn. Represent., 2019.

4.Pengju Liu, Hongzhi Zhang, Kai Zhang, Liang Lin, and Wangmeng Zuo. Multi-level wavelet-cnn for image restoration. In Proc. IEEE Conf. Comput. Vis. Pattern Recog. Worksh., pages 886–88609, 2018.（**基于小波变换**）

**未知质量因素的恢复（blind restoration）**



### DCT域和像素域的方法

1.Jun Guo and Hongyang Chao, “Building dual-domain representations for compression artifacts reduction,” in Proceedings of the European Conference on Computer Vision. Springer, 2016, pp. 628–644.（无源码）

（DCNN）

2.Dmcnn: Dual-domain multi-scale convolutional neural network for compression artifacts removal.2018（无源码）

笔记：https://github.com/Qinluyi/compressed-image-restoration/blob/main/jpeg_paper/DMCNN.pptx

3.Implicit dual-domain convolutional network for robust color image compression artifact reduction.（无源码）

4.Zhangyang Wang et al. “D3: Deep dual-domain based fast restoration of jpegcompressed images”. In: Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. 2016, pp. 2764–2772.（无源码）

5.Zhi Jin et al. “Dual-stream Multi-path Recursive Residual Network for JPEG Image Compression Artifacts Reduction”. In: IEEE Transactions on Circuits and Systems for Video Technology (2020).

### DCT域的方法

1.Max Ehrlich, Larry Davis, Ser-Nam Lim, and Abhinav Shrivastava. Quantization guided jpeg artifact correction. In Proc. Eur. Conf. Comput. Vis., Glasgow, UK, pages 293–309. Springer, 2020.（QGAC）

# general image restoration的方法

1.Yulun Zhang et al. “Residual dense network for image restoration”. In: IEEE Transactions on Pattern Analysis and Machine Intelligence (2020).





