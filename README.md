# COCO-annotations_convert from @ujsyehao
This repository is a copy of @ujsyehao script but with all the corrections mentionned in his issues.

## Corrections
- Script error : "Filter object is not subscriptable"
  - [Pull request with solution](https://github.com/ujsyehao/COCO-annotations-darknet-format/pull/3)

- Solution to [Issue#1](https://github.com/ujsyehao/COCO-annotations-darknet-format/issues/1)
  - added solution by [**@florazxf**](https://github.com/florazxf) [here](https://github.com/ujsyehao/COCO-annotations-darknet-format/issues/1#issuecomment-643747299)

## Original
COCO just provide json file annotations. If you want to train COCO on darknet,thie program can help you turn json file into txt 
file that darknet need.

you should download COCO dataset and annotations from http://mscoco.org/dataset/.

tips you should know about COCO dataset:

1. COCO have three types of annotations including captions,keypoints and instances. we just use instances annotations to have 
bounding boxes in the image.

2. The annotations file including image_info_test2014/2015.json,image_info_test-dev2015.json,instances_train2014/val2014.json.
and we just use instances_train2014/val2014.json，the other three annotation files just have image paths and don't have bounding boxes.

3. Information about instances_train2014/val2014.json,you should look at the COCO website.


## pascal-to-coco format
provide script **coco_format_yehao.py**
