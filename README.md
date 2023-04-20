# PointCloudProcessDemo
點雲基本處理範例程式
主要的點雲處理套件: pdal, pyproj, laspy, numba, CSF 
若安裝上有問題可以直接詢問我

##  Step1.crop_outlier.ipynb
可先將原始點雲用GUI工具開啟看看，可以發現原本的點雲可能因為極少的造訊點有非常大的範圍是被浪費的。
在此程式主要是處理將點雲資料的讀取後，篩選出我們所需要的資訊並寫出成另一份點雲檔。

##  Step2.Ground_Filter.ipynb
此程式為利用Cloth Simulation Filter (CSF)來擷取點雲中的地面點及非地面點的處理，可參考
1. [CloudCompare Plugin](https://www.cloudcompare.org/doc/wiki/index.php?title=CSF_(plugin))
2. Source Code: [Github](https://github.com/jianboqi/CSF)
<img src="https://i.imgur.com/YN0ow8k.png" data-canonical-src="https://i.imgur.com/YN0ow8k.png" width="350" height="200" />
可分解成
<img src="https://i.imgur.com/DvmiXfq.png" data-canonical-src="https://i.imgur.com/DvmiXfq.png" width="350" height="200" />  +  <img src="https://i.imgur.com/PRmMfLP.png" data-canonical-src="https://i.imgur.com/PRmMfLP.png" width="350" height="200" />
