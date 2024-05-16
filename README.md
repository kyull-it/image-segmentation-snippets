# Image Segmentation

[OXFORD-IIIT-PET](https://www.robots.ox.ac.uk/%7Evgg/data/pets/) 데이터셋을 파악하기 위해서 sample_code.ipynb를 작성하였습니다.

* xml annotation을 파싱하여 bounding box를 시각화
* pixel annotation인 trimap을 이용하여 foreground, background, unknown을 시각화


### 어노테이션 예시

1. list.txt

```
IMAGE   CLASS-ID    SPECIES BREED-ID
 
 Abyssinian_100     1   1   1
 basset_hound_137   4   2   3
```

2. xmls/*.xml

```xml
<annotation>
	<folder>
	  OXIIIT
	</folder>
	<filename>
	  Abyssinian_1.jpg
	</filename>
	<source>
		<database>
		  OXFORD-IIIT Pet Dataset
		</database>
		<annotation>
		  OXIIIT
		</annotation>
		<image>
		  flickr
		</image>
	</source>
	<size>
		<width>
		  600
		</width>
		<height>
		  400
		</height>
		<depth>
		  3
		</depth>
	</size>
	<segmented>
	  0
	</segmented>
	<object>
		<name>
		  cat
		</name>
		<pose>
		  Frontal
		</pose>
		<truncated>
		  0
		</truncated>
		<occluded>
		  0
		</occluded>
		<bndbox>
			<xmin>
			  333
			</xmin>
			<ymin>
			  72
			</ymin>
			<xmax>
			  425
			</xmax>
			<ymax>
			  158
			</ymax>
		</bndbox>
		<difficult>
		  0
		</difficult>
	</object>
</annotation>
```
