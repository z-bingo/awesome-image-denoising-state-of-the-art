## Awesome Image or Video Denoising Algorithms
Collection of popular and reproducible image denoising works.

**I will update the document when I access the new work for image or video denoising. Everyone could pull requests or remind me to update if you access the latest work.**

This collection is based on the summary of [wenbihan's work](https://github.com/wenbihan/reproducible-image-denoising-state-of-the-art).

## Contents
1. [Denoising Algorithms](#denoising-algorithms)  
    1.1 [Filter](#filter)  
    1.2 [Sparse Coding](#sparse-coding)  
    1.3 [Effective Prior](#effective-prior)  
    1.4 [Low Rank](#low-rank)  
    1.5 [Deep Learning](#deep-learning)  
    1.6 [Sparsity and Low-rankness Combined](#sparsity-and-low-rankness-combined)  
    1.7 [Combined with High-Level Tasks](#combined-with-high-level-tasks)  
    1.8 [Image Noise Level Estimation](#image-noise-level-estimation)
2. [Benchmark and Dataset](#benchmark-and-dataset)  
    2.1 [Novel Benchmark](#novel-benchmark)  
    2.2 [Commonly Used Denoising Dataset](#commonly-used-denoising-dataset)
3. [Others](#others)  
    3.1 [Commonly Used Image Quality Metric Code](#commonly-used-image-quality-metric-code)

## Denoising Algorithms
#### Filter
 * NLM [[Web]](https://sites.google.com/site/shreyamsha/publications/image-denoising-based-on-nlfmt) [[Code]](https://www.mathworks.com/matlabcentral/fileexchange/44090-image-denoising-based-on-non-local-means-filter-and-its-method-noise-thresholding?focused=3806802&tab=function) [[PDF]](https://link.springer.com/article/10.1007/s11760-012-0389-y)
   * A non-local algorithm for image denoising (CVPR 05), Buades et al.
   * Image denoising based on non-local means filter and its method noise thresholding (SIVP2013), B. Kumar
 * BM3D [[Web]](http://www.cs.tut.fi/~foi/GCF-BM3D/) [[Code]](http://www.cs.tut.fi/~foi/GCF-BM3D/BM3D.zip) [[PDF]](http://www.cs.tut.fi/~foi/GCF-BM3D/SPIE08_deblurring.pdf)
   * Image restoration by sparse 3D transform-domain collaborative filtering (SPIE Electronic Imaging 2008), Dabov et al.   
 * PID [[Web]](http://www.cgg.unibe.ch/publications/progressive-image-denoising) [[Code]](http://www.cgg.unibe.ch/publications/progressive-image-denoising/pid.zip) [[PDF]](http://www.cgg.unibe.ch/publications/2014/progressive-image-denoising/at_download/file)
   * Progressive Image Denoising (TIP 2014), C. Knaus et al.

#### Sparse Coding
 * KSVD [[Web]](http://www.cs.technion.ac.il/~ronrubin/software.html) [[Code]](https://github.com/jbhuang0604/SelfSimSR/tree/master/Lib/KSVD) [[PDF]](http://www.egr.msu.edu/~aviyente/elad06.pdf)
   * Image Denoising Via Sparse and Redundant Representations Over Learned Dictionaries (TIP 2006), Elad et al.
 * LSSC [[Web]](https://lear.inrialpes.fr/people/mairal/) [[Code]](https://lear.inrialpes.fr/people/mairal/resources/denoise_ICCV09.tar.gz) [[PDF]](http://www.di.ens.fr/~fbach/iccv09_mairal.pdf)
   * Non-local Sparse Models for Image Restoration (ICCV 2009), Mairal et al.
 * NCSR [[Web]](http://www4.comp.polyu.edu.hk/~cslzhang/NCSR.htm) [[Code]](http://www4.comp.polyu.edu.hk/~cslzhang/code/NCSR.rar) [[PDF]](http://www4.comp.polyu.edu.hk/~cslzhang/paper/NCSR_TIP_final.pdf)
   * Nonlocally Centralized Sparse Representation for Image Restoration (TIP 2012), Dong et al.  
 * OCTOBOS [[Web]](http://transformlearning.csl.illinois.edu/projects/) [[Code]](https://github.com/wenbihan/octobos_IJCV2016) [[PDF]](http://transformlearning.csl.illinois.edu/assets/Sai/JournalPapers/SaiBihanIJCV2014OCTOBOS.pdf)
   * Structured Overcomplete Sparsifying Transform Learning with Convergence Guarantees and Applications (IJCV 2015), Wen et al. 
 * GSR [[Web]](https://jianzhang.tech/projects/GSR/) [[Code]](http://csjianzhang.github.io/codes/GSR_Code_Package_3.0.zip) [[PDF]](http://csjianzhang.github.io/papers/TIP2014_single.pdf)
   * Group-based Sparse Representation for Image Restoration (TIP 2014), Zhang et al.
 * TWSC [[Web]](https://github.com/csjunxu/TWSC-ECCV2018) [[Code]](https://github.com/csjunxu/TWSC-ECCV2018) [[PDF]](http://openaccess.thecvf.com/content_ECCV_2018/papers/XU_JUN_A_Trilateral_Weighted_ECCV_2018_paper.pdf)
   * A Trilateral Weighted Sparse Coding Scheme for Real-World Image Denoising (ECCV 2018), Xu et al.
  
#### Effective Prior
 * EPLL [[Web]](https://people.csail.mit.edu/danielzoran/) [[Code]](https://people.csail.mit.edu/danielzoran/epllcode.zip) [[PDF]](http://people.ee.duke.edu/~lcarin/EPLICCVCameraReady.pdf)
   * From Learning Models of Natural Image Patches to Whole Image Restoration (ICCV2011), Zoran et al.
 * GHP [[Web]][[Code]](https://github.com/tingfengainiaini/GHPBasedImageRestoration) [[PDF]](https://www.cv-foundation.org/openaccess/content_cvpr_2013/papers/Zuo_Texture_Enhanced_Image_2013_CVPR_paper.pdf)
   * Texture Enhanced Image Denoising via Gradient Histogram Preservation (CVPR2013), Zuo et al.
 * PGPD [[Web]][[Code]](https://github.com/csjunxu/PGPD_Offline_BID) [[PDF]](http://www4.comp.polyu.edu.hk/~cslzhang/paper/PGPD.pdf)
   * Patch Group Based Nonlocal Self-Similarity Prior Learning for Image Denoising (ICCV 2015), Xu et al.
 * PCLR [[Web]][[Code]](http://www4.comp.polyu.edu.hk/~cslzhang/code/PCLR.zip) [[PDF]](http://www4.comp.polyu.edu.hk/~cslzhang/paper/PCLR.pdf)
   * External Patch Prior Guided Internal Clustering for Image Denoising (ICCV 2015), Chen et al.
   
#### Low Rank
 * SAIST [[Web]](http://see.xidian.edu.cn/faculty/wsdong/wsdong_Publication.htm) [Code by request] [[PDF]](http://see.xidian.edu.cn/faculty/wsdong/Papers/Journal/TIP_LASSC.pdf)
   * Nonlocal image restoration with bilateral variance estimation: a low-rank approach (TIP2013), Dong et al.
 * WNNM [[Web]](https://sites.google.com/site/shuhanggu/home) [[Code]](http://www4.comp.polyu.edu.hk/~cslzhang/code/WNNM_code.zip) [[PDF]](https://pdfs.semanticscholar.org/6d55/6272625b672ba54b5ab3d9e6474088a4b78f.pdf)
   * Weighted Nuclear Norm Minimization with Application to Image Denoising (CVPR2014), Gu et al.
 * Multi-channel WNNM [[Web]](http://www4.comp.polyu.edu.hk/~csjunxu/Publications.html) [[Code]](http://www4.comp.polyu.edu.hk/~csjunxu/code/MCWNNM.zip) [[PDF]](http://www4.comp.polyu.edu.hk/~csjunxu/paper/MCWNNM.pdf)
   * Multi-channel Weighted Nuclear Norm Minimization for Real Color Image Denoising (ICCV 2017), Xu et al.
   
#### Deep Learning
 * SF [[Web]](http://www.visinf.tu-darmstadt.de/vi_research/code/index.en.jsp#shrinkage_fields) [[Code]](https://github.com/uschmidt83/shrinkage-fields) [[PDF]](http://research.uweschmidt.org/pubs/cvpr14schmidt.pdf)
   * Shrinkage Fields for Effective Image Restoration (CVPR 2014), Schmidt et al.
   
 * TNRD [[Web]](http://www.icg.tugraz.at/Members/Chenyunjin/about-yunjin-chen) [[Code]](https://www.dropbox.com/s/8j6b880m6ddxtee/TNRD-Codes.zip?dl=0) [[PDF]](https://arxiv.org/pdf/1508.02848.pdf)
   * Trainable nonlinear reaction diffusion: A flexible framework for fast and effective image restoration (TPAMI 2016), Chen et al.
   
 * RED [[Web]](https://bitbucket.org/chhshen/image-denoising/) [[Code]](https://bitbucket.org/chhshen/image-denoising/) [[PDF]](https://arxiv.org/pdf/1603.09056.pdf)
   * Image Restoration Using Very Deep Convolutional Encoder-Decoder Networks with Symmetric Skip Connections (NIPS2016), Mao et al.
   
 * DnCNN [[Web]](https://github.com/cszn/DnCNN) [[Code]](https://github.com/cszn/DnCNN) [[PDF]](https://arxiv.org/pdf/1608.03981v1.pdf)
   * Beyond a Gaussian Denoiser: Residual Learning of Deep CNN for Image Denoising (TIP2017), Zhang et al.
   
 * MemNet [[Web]](https://github.com/tyshiwo/MemNet) [[Code]](https://github.com/tyshiwo/MemNet) [[PDF]](http://cvlab.cse.msu.edu/pdfs/Image_Restoration%20using_Persistent_Memory_Network.pdf)
   * MemNet: A Persistent Memory Network for Image Restoration (ICCV2017), Tai et al.  
   
 * WIN [[Web]](https://github.com/cswin/WIN) [[Code]](https://github.com/cswin/WIN) [[PDF]](https://arxiv.org/pdf/1707.09135.pdf)
   * Learning Pixel-Distribution Prior with Wider Convolution for Image Denoising (Arxiv), Liu et al.    
   
 * F-W Net [[Web]](https://github.com/sunke123/FW-Net) [[Code]](https://github.com/sunke123/FW-Net) [[PDF]](https://arxiv.org/abs/1802.10252)
   * L_p-Norm Constrained Coding With Frank-Wolfe Network (Arxiv), Sun et al.
   
 * NLCNN [[Web]](https://cig.skoltech.ru/publications) [[Code]](https://github.com/cig-skoltech/NLNet) [[PDF]](http://www.skoltech.ru/app/data/uploads/sites/19/2017/06/1320.pdf)
   * Non-Local Color Image Denoising with Convolutional Neural Networks (CVPR 2017), Lefkimmiatis.

 * Deep image prior [[Web]](https://dmitryulyanov.github.io/deep_image_prior) [[Code]](https://github.com/DmitryUlyanov/deep-image-prior) [[PDF]](https://sites.skoltech.ru/app/data/uploads/sites/25/2018/04/deep_image_prior.pdf)
   * Deep Image Prior (CVPR 2018), Ulyanov et al.
   
 * xUnit [[Web]](https://github.com/kligvasser/xUnit) [[Code]](https://github.com/kligvasser/xUnit) [[PDF]](https://arxiv.org/pdf/1711.06445.pdf)
   * xUnit: Learning a Spatial Activation Function for Efficient Image Restoration (Arxiv), Kligvasser et al.  
   
 * UDNet [[Web]](https://github.com/cig-skoltech/UDNet) [[Code]](https://github.com/cig-skoltech/UDNet) [[PDF]](https://arxiv.org/pdf/1711.07807.pdf)
   * Universal Denoising Networks : A Novel CNN Architecture for Image Denoising (CVPR 2018), Stamatios  Lefkimmiatis.   
   
 * Wavelet-CNN [[Web]](https://github.com/lpj0/MWCNN) [[Code]](https://github.com/lpj0/MWCNN) [[PDF]](https://arxiv.org/abs/1805.07071)
   * Multi-level Wavelet-CNN for Image Restoration (Arxiv), Liu et al.  
   
 * FFDNet [[Web]](https://github.com/cszn/FFDNet/) [[Code]](https://github.com/cszn/FFDNet/) [[PDF]](https://arxiv.org/abs/1710.04026)
   * FFDNet: Toward a Fast and Flexible Solution for CNN-Based Image Denoising (TIP), Zhang et al.
   
 * FC-AIDE [[Web]](https://github.com/csm9493/FC-AIDE) [[Code]](https://github.com/GuoShi28/CBDNet) [[PDF]](https://arxiv.org/pdf/1807.07569.pdf)
   * Fully Convolutional Pixel Adaptive Image Denoiser (Arxiv), Cha et al. 
    
 * CBDNet [[Web]](https://github.com/GuoShi28/CBDNet) [[Code]](https://github.com/GuoShi28/CBDNet) [[PDF]](https://arxiv.org/pdf/1807.04686.pdf)
   * Toward Convolutional Blind Denoising of Real Photographs (Arxiv), Guo et al.  
   
 * Noise2Noise [[Web]](https://github.com/yu4u/noise2noise) [[TF Code]](https://github.com/NVlabs/noise2noise) [[Keras Unofficial Code]](https://github.com/yu4u/noise2noise) [[PDF]](https://arxiv.org/pdf/1803.04189.pdf)
   * Noise2Noise: Learning Image Restoration without Clean Data (ICML 2018), Lehtinen et al.

 * Neighbor2Neighbor [[Official Code]](https://github.com/TaoHuang2018/Neighbor2Neighbor) [[Minimal PyTorch Code]](https://github.com/neeraj3029/Ne2Ne-Image-Denoising) [[PDF]](https://arxiv.org/abs/2101.02824.pdf)
   * Neighbor2Neighbor: Self-Supervised Denoising from Single Noisy Images, Huang et al.      
   
 * UDN [[Web]](https://cig.skoltech.ru/publications) [[Code]](https://github.com/cig-skoltech/UDNet) [[PDF]](http://www.skoltech.ru/app/data/uploads/sites/19/2018/03/UDNet_CVPR2018.pdf)
   * Universal Denoising Networks- A Novel CNN Architecture for Image Denoising (CVPR 2018), Lefkimmiatis.     
   
 * N3 [[Web]](https://github.com/visinf/n3net) [[Code]](https://github.com/visinf/n3net) [[PDF]](https://arxiv.org/abs/1810.12575)
   * Neural Nearest Neighbors Networks (NIPS 2018), Plotz et al.  
   
 * NLRN [[Web]](https://github.com/Ding-Liu/NLRN) [[Code]](https://github.com/Ding-Liu/NLRN) [[PDF]](https://arxiv.org/pdf/1806.02919.pdf)
   * Non-Local Recurrent Network for Image Restoration (NIPS 2018), Liu et al.
   
 * KPN [[Web]]() [[Code]]() [[PDF]](https://arxiv.org/pdf/1712.02327.pdf)
   * Burst Denoising with Kernel Prediction Networks (CVPR 2018), Ben et al.
   
 * MKPN [[Web]]() [[Code]]() [[PDF]](https://arxiv.org/pdf/1902.05392.pdf)
   * Multi-Kernel Prediction Networks for Denoising of Burst Images (ArXiv 2019), Marinc et al.
   
 * RFCN [[Web]](http://visual.cs.ucl.ac.uk/pubs/deepBurstDenoising/) [[Code]]() [[PDF]](https://arxiv.org/pdf/1712.05790.pdf) [[PDF]](https://arxiv.org/pdf/1904.07483.pdf)
   * Deep Burst Denoising (ArXiv 2017), Clement et al.
   * End-to-End Denoising of Dark Burst Images Using Recurrent Fully Convolutional Networks (ArXiv 2019), Zhao et al.
   
 * CNN-LSTM [[Web]]() [[Code]]() [[PDF]](https://arxiv.org/pdf/1801.05141.pdf)
   * Image denoising and restoration with CNN-LSTM Encoder Decoder with Direct Attention (ArXiv 2018), Haque et al.
   
 * GRDN [[Web]]() [[Code]]() [[PDF]](https://arxiv.org/pdf/1905.11172.pdf)
   * GRDN: Grouped Residual Dense Network for Real Image Denoising and GAN-based Real-world Noise Modeling (CVPR 2019), Kim et al.
   
 * Deformable KPN [[Web]]() [[Code]]() [[PDF]](https://arxiv.org/pdf/1904.06903.pdf)
   * Learning Deformable Kernels for Image and Video Denoising (ArXiv 2019), Xu et al.

 * BayerUnify BayerAug [[Web]]() [[Code]](https://github.com/Jiaming-Liu/BayerUnifyAug) [[PDF]](http://openaccess.thecvf.com/content_CVPRW_2019/papers/NTIRE/Liu_Learning_Raw_Image_Denoising_With_Bayer_Pattern_Unification_and_Bayer_CVPRW_2019_paper.pdf)
   * Learning Raw Image Denoising With Bayer Pattern Unification and Bayer Preserving Augmentation (CVPR 2019), Liu et al.
 
 * RDU-UD [[Web]]() [[Code]]() [[PDF]](http://openaccess.thecvf.com/content_CVPRW_2019/papers/NTIRE/Sim_A_Deep_Motion_Deblurring_Network_Based_on_Per-Pixel_Adaptive_Kernels_CVPRW_2019_paper.pdf)
   * A Deep Motion Deblurring Network Based on Per-Pixel Adaptive Kernels With Residual Down-Up and Up-Down Modules (CVPR 2019), Sim et al.
 
 * RIDNet [[Web]]() [[Code]]() [[PDF]](https://arxiv.org/pdf/1904.07396.pdf)
   * Real Image Denoising with Feature Attention (ArXiv 2019), Anwar et al.
 
 * EDVR [[Web]](https://github.com/xinntao/EDVR) [[Code]](https://github.com/xinntao/EDVR) [[PDF]](http://openaccess.thecvf.com/content_CVPRW_2019/papers/NTIRE/Wang_EDVR_Video_Restoration_With_Enhanced_Deformable_Convolutional_Networks_CVPRW_2019_paper.pdf)
   * EDVR: Video Restoration With Enhanced Deformable Convolutional Networks (CVPR 2019), Wang et al.
   
 * DVDNet[[Web]](https://github.com/m-tassano/dvdnet) [[Code]](https://github.com/m-tassano/dvdnet) [[PDF]](https://arxiv.org/pdf/1906.11890.pdf)
   * DVDnet: A Fast Network for Deep Video Denoising (ArXiv 2019), Tassano et al.
 
 * FastDVDNet [[Web]](https://github.com/m-tassano/fastdvdnet) [[Code]](https://github.com/m-tassano/fastdvdnet) [[An Unofficial PyTorch Code]](https://github.com/z-bingo/FastDVDNet) [[PDF]](https://arxiv.org/pdf/1907.01361.pdf)
   * FastDVDnet: Towards Real-Time Video Denoising Without Explicit Motion Estimation (ArXiv 2019), Tassano et al.
   
 * ViDeNN [[Web]]() [[Code]]() [[PDF]](https://arxiv.org/pdf/1904.10898.pdf)
   * ViDeNN: Deep Blind Video Denoising (ArXiv 2019), Calus et al.
  
 * Multi-Level Wavelet-CNN [[Web]]() [[Code]]() [[PDF]](https://arxiv.org/pdf/1907.03128.pdf)
   * Multi-Level Wavelet Convolutional Neural Networks (IEEE Access), Liu et al.
   
 * PRIDNet [[Web]]() [[Code]]() [[PDF]](https://arxiv.org/pdf/1908.00273.pdf)
   * Pyramid Read Image Denoising Network (Arxiv 2019), Zhao et al.
   
 * CycleISP [[Web]](https://github.com/swz30/CycleISP) [[Code]](https://github.com/swz30/CycleISP) [[PDF]](https://arxiv.org/pdf/2003.07761.pdf)
   * CycleISP: Real Image Restoration via Improved Data Synthesis (CVPR 2020), Zamir et al.
   
 * MIRNEt [[Web]](https://github.com/swz30/MIRNet) [[Code]](https://github.com/swz30/MIRNet) [[PDF]](https://arxiv.org/pdf/2003.06792.pdf)
   * MIRNEt: Learning Enriched Features for Real Image Restoration and Enhancement (ECCV 2020), Zamir et al.
   
 
#### Sparsity and Low-rankness Combined
 * STROLLR-2D [[PDF]](http://transformlearning.csl.illinois.edu/assets/Bihan/ConferencePapers/BihanICASSP2017strollr.pdf) [[Code]](https://github.com/wenbihan/strollr2d_icassp2017) 
   * When Sparsity Meets Low-Rankness: Transform Learning With Non-Local Low-Rank Constraint for Image Restoration (ICASSP 2017), Wen et al.
   
#### Combined with High-Level Tasks
 * Meets High-level Tasks [[PDF]](https://arxiv.org/pdf/1706.04284.pdf) [[Code]](https://github.com/wenbihan/DeepDenoising) 
   * When Image Denoising Meets High-Level Vision Tasks: A Deep Learning Approach (IJCAI 2018), Liu et al.

#### Diffusion-Based Models
 * Denoising-ODE [[Code]](https://github.com/Algolzw/image-restoration-sde) [[PDF]](https://arxiv.org/pdf/2301.11699) [[Project]](https://algolzw.github.io/ir-sde/index.html)
    * Image Restoration with Mean-Reverting Stochastic Differential Equations (ICML 2023), Luo et al.

#### Image Noise Level Estimation
 * SINLE [[PDF]](http://www.ok.sc.e.titech.ac.jp/res/NLE/TIP2013-noise-level-estimation06607209.pdf) [[Code]](https://www.mathworks.com/matlabcentral/fileexchange/36921-noise-level-estimation-from-a-single-image) [[Slides]](https://wwwpub.zih.tu-dresden.de/~hh3/Hauptsem/SS16/noise.pdf)
   * Single-image Noise Level Estimation for Blind Denoising (TIP 2014), Liu et al.
 * CBDNet [[Code]](https://github.com/GuoShi28/CBDNet) [[PDF]](https://arxiv.org/pdf/1807.04686.pdf)
   * Toward Convolutional Blind Denoising of Real Photographs (Arxiv), Guo et al.
 * HyperIQA [[Code]](https://github.com/SSL92/hyperIQA) [[PDF]](https://openaccess.thecvf.com/content_CVPR_2020/papers/Su_Blindly_Assess_Image_Quality_in_the_Wild_Guided_by_a_CVPR_2020_paper.pdf)
   * Blindly Assess Image Quality in the Wild Guided by A Self-Adaptive Hyper Network (CVPR 2020), Su et al.
 * PaQ-2-PiQ [[Code]](https://github.com/baidut/PaQ-2-PiQ) [[PDF]](https://arxiv.org/pdf/1912.10088.pdf)
   * From Patches to Pictures (PaQ-2-PiQ): Mapping the Perceptual Space of Picture Quality (Arxiv), Ying et al.

## Benchmark and Dataset
#### Novel Benchmark
 * ReNOIR [[Web]](http://ani.stat.fsu.edu/~abarbu/Renoir.html) [[Data]](http://ani.stat.fsu.edu/~abarbu/Renoir.html) [[PDF]](https://arxiv.org/pdf/1409.8230.pdf)
   * RENOIR - A Dataset for Real Low-Light Image Noise Reduction (Arxiv 2014), Anaya, Barbu.   
 * PolyU [[Web]](https://github.com/csjunxu/PolyU-Real-World-Noisy-Images-Dataset) [[Data]](https://github.com/csjunxu/PolyU-Real-World-Noisy-Images-Dataset) [[PDF]](https://arxiv.org/pdf/1804.02603.pdf)
   * Real-world Noisy Image Denoising: A New Benchmark (Arxiv), Xu et al.
 * Nam [[Web]](http://snam.ml/research/ccnoise) [[PDF]](http://snam.ml/assets/ccnoise_cvpr16/ccnoise_cvpr16.pdf)
   * A Holistic Approach to Cross-Channel Image Noise Modeling and its Application to Image Denoising (CVPR 2016), Nam et al.
 * Darmstadt (DND) [[Web]](https://noise.visinf.tu-darmstadt.de/) [[Data]](https://noise.visinf.tu-darmstadt.de/downloads/) [[PDF]](https://download.visinf.tu-darmstadt.de/papers/2017-cvpr-ploetz-benchmarking_denoising_algorithms-preprint.pdf)
   * Benchmarking Denoising Algorithms with Real Photographs (CVPR 2017), Plotz et al.
 * SIDD [[Web]](https://www.eecs.yorku.ca/~kamel/sidd/dataset.php)
   * A High-Quality Denoising Dataset for Smartphone Cameras.
   
#### Commonly Used Denoising Dataset
 * Kodak [[Web]](http://r0k.us/graphics/kodak/)
 * USC SIPI-Misc [[Web]](http://sipi.usc.edu/database/database.php?volume=misc) 
 * BSD [[Web]](https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/bsds/)  
 * Vimeo-90K [[Web]](http://toflow.csail.mit.edu/)
 * Adobe-5K [[Web]](https://data.csail.mit.edu/graphics/fivek/)
 * OpenImage [[Web]](http://storage.googleapis.com/openimages/web/index.html)

## Others
#### Commonly Used Image Quality Metric Code
 * PSNR (Peak Signal-to-Noise Ratio) [[Wiki]](https://en.wikipedia.org/wiki/Peak_signal-to-noise_ratio) [[Matlab Code]](https://www.mathworks.com/help/images/ref/psnr.html) [[Python Code]](https://github.com/aizvorski/video-quality) [[PyTorch Code]](https://github.com/z-bingo/FastDVDNet/blob/master/utils/data_utils.py#L13)
 
 * SSIM (Structural similarity) [[Wiki]](https://en.wikipedia.org/wiki/Structural_similarity) [[Matlab Code]](http://www.cns.nyu.edu/~lcv/ssim/ssim_index.m) [[Python Code]](https://github.com/aizvorski/video-quality/blob/master/ssim.py) [[PyTorch Code]](https://github.com/z-bingo/FastDVDNet/blob/master/utils/data_utils.py#L26)
 
 * NIQE (Naturalness Image Quality Evaluator) [[Web]](http://live.ece.utexas.edu/research/Quality/nrqa.htm) [[Matlab Code]](http://live.ece.utexas.edu/research/Quality/nrqa.htm) [[Python Code]](https://github.com/aizvorski/video-quality/blob/master/niqe.py)



   
