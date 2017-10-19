# Image Fusion of Hyperspectral Data and Panchromatic Data 
## Main idea
ALI and Hyperion data are data acquired through ALI (Advanced Land Imager) and spectral imaging spectrometer (Hyperion) on Earth observation satellites -1 (EO-1). These two products are able to meet the requirements of many remote sensing tasks.

Multi-spectral and hyperspectral images:
* pros: high spectral resolution
* cons: limited spatial resolution

ALI Panchromatic images:
* pros: high spatial resolution
* cons: low spectral resolution

The fusion of ALI panchromatic with multispectral data and fusion of Hyperion data with panchromatic data can effectively improve the quality of data to meet the needs of practical application, while the spectral characteristics and spectral shape can selectively retain from the original image. 

## Methods
* HSV transform, Brovey transform and Gram-Schmidt transform are applied to fusion of ALI panchromatic image and multispectral image.<br><br>

* Principal component analysis (PCA) and Non-negative matrix factorization are applied to fusion of ALI panchromatic image and Hyperion image. <br><br>

Non-negative matrix factorization: unmix pixel of hyperion image with provided endmember info, added with spatial info created by high-pass filter from ALI panchromatic image.
<br><br>
Entropy, Average Gradient, Correlation coefficient and PSNR(Peak signal-to-noise ratio) could be used to evaluate the fusion.

## Source
ALI (res: 10m), Hyperion data (res: 30m) of the Yellow River Delta in 2005

## Results
* Images have been clipped with Taihu Lake shapefile
* Pixel value ranges from -1 to 1 (NDVI range), while higher value represents higher concentration of vegetation theoretically.
* Image is scaled with -1 as black and 1 as white.
* Stripes of 2007 image are caused by sensor malfunction.
<div align=center><img width="300" height="300" src="https://github.com/acephaly/PNG-Files/blob/master/2004.png?raw=true"><img align="left" width="300" height="300" src="https://github.com/acephaly/PNG-Files/blob/master/2003.png?raw=true" style="float: left"></div>
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;2003 &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;  &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;  2004
<br> <br>
<div align=center><img width="300" height="300" src="https://github.com/acephaly/PNG-Files/blob/master/2006.png?raw=true"><img align="left" width="300" height="300" src="https://github.com/acephaly/PNG-Files/blob/master/2005.png?raw=true" style="float: left"></div>
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;2005 &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;  &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;  2006
<br> <br>
<div align=center><img width="300" height="300" src="https://github.com/acephaly/PNG-Files/blob/master/2008.png?raw=true"><img align="left" width="300" height="300" src="https://github.com/acephaly/PNG-Files/blob/master/2007.png?raw=true" style="float: left"></div>
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;2007 &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;  &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;  2008
<br> <br>
<div align=center><img width="300" height="300" src="https://github.com/acephaly/PNG-Files/blob/master/2010.png?raw=true"><img align="left" width="300" height="300" src="https://github.com/acephaly/PNG-Files/blob/master/2009.png?raw=true" style="float: left"></div>
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;2009 &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;  &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;  2010
<br> <br>
<img align="left" width="300" height="300" src="https://github.com/acephaly/PNG-Files/blob/master/2011.png?raw=true" style="float: left">
<br><br><br><br><br><br><br><br><br><br><br><br>
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;2011 &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;  &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp;  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;
<br> <br>
