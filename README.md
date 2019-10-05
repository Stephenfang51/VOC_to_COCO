# VOC_to_COCO

> update 2019.10.5



最简单的VOC数据集转换为COCO数据集方式

修改路径后， **只要一条指令就能转换** 





1. 请先确认你的VOC如下面的格式

   ```
     VOC
       |-- Annotations
       		|-- all xml files
       |-- JPEGImages
       		|-- all your samples
       |-- ImageSets
       		|-- 。。。。
   
   ```



2. 克隆本仓到你指定的地址

   `git clone https://github.com/Stephenfang51/VOC_to_COCO `



3. cd 到VOC_to_COCO 编辑 voc_to_coco.py修改以下3点

   1. 设定验证集样本数
   2. 设定测试集样本数
   3. VOC Annotations 资料夹路径（最后面的"/"务必加上， 否则报错）

   例如

   ```python3
   val_files_num = 100
   test_files_num = 100
   voc_annotations = '././VOC/Annotations/'  #remember to modify the path
   ```

   修改到这边已经结束

4. 执行生成

   ```
   python3 voc_to_coco.py
   ```

   

5. COCO 数据集已经生成与VOC同一主目录下
