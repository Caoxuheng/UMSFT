<img align="right" src="https://ars.els-cdn.com/content/image/X00303992.jpg" width="290" height="350"/>  

# Unsupervised Multi-level Spatio-spectral Fusion Transformer for Hyperspectral Image Super-resolution
Fusing a low spatial resolution hyperspectral image (LR-HSI) with a high spatial resolution multispectral image (HR-MSI) is widely used for HSI super-resolution. Recent works still face problems in exploring global spatio-spectral correlation and lack effective utilization of multi-level features of the inputs (i.e., HR-MSI and LR-HSI), which results in a lack of similarity between the reconstruction and the inputs, ultimately causing significant spatio-spectral distortion. To solve these problems, we design an Unsupervised Multi-level Spatio-spectral Fusion Transformer (UMSFT). In UMSFT, a novel multi-level features fusion strategy is constructed, which fuses the hierarchy features of the inputs via proposed Spatio-spectral Feature Fusion Attention Blocks (S2F-FAB) in a level-by-level manner, thereby fully exploring the interaction between the hierarchical features. The S2F-FAB is specially designed for HSI-MSI fusion consisting of two components: (1) a spatial fusion module (Spa-FM) is designed for spatial domain fusion, and its output is set as Values (V) of a transformer; (2) a novel spectral feature cross attention (Spe- FCA) formulates the features of LR-HSI and HR-MSI as Queries (Q) and Keys (K), respectively, and achieves spectral domain fusion by applying attention mechanism along the spectral dimension. Incorporating spatial detail reconstruction and spectral feature integration into the attention mechanism, the S2F-FAB efficiently exploits the spatio-spectral correlation between target HR-HSI and inputs. Experimental results on three public datasets and our real-world images show the superiority of our method as compared with eleven state-of-the-art methods.   

# Flowchart
**None**
# Result presentation
![Performance](https://github.com/Caoxuheng/imgs/blob/main/%E5%9B%BE%E7%89%871.png)  
The reconstructed results can be downloaded from [`here`](https://aistudio.baidu.com/aistudio/datasetdetail/182575).
# Guidance

# Requirements
## Environment
`Python3.8`  
`torch 1.12`,`torchvision 0.13.0`  
`Numpy`,`Scipy`  
*Also, we will create a Paddle version that implements FeafusFormer in AI Studio online for free!*
## Datasets
[`CAVE dataset`](https://www1.cs.columbia.edu/CAVE/databases/multispectral/), 
 [`Preprocessed CAVE dataset`](https://aistudio.baidu.com/aistudio/datasetdetail/147509).
# Note
For any questions, feel free to email me at caoxuhengcn@gmail.com.  
If you find our work useful in your research, please cite our paper ^.^
