# Official JutePest-YOLO

Implementation of paper - [JutePest-YOLO: A Deep Learning Network for
Jute Pest Identification and Detection](https://doi.org/10.1109/ACCESS.2024.3403491)



## Testing

``` shell
python test.py --data data/data.yaml --img 640 --batch 32 --conf 0.001 --iou 0.65 --device 0 --weights JutePest-YOLO.pt --name JutePest-YOLO_640_val
```



## Training

Single GPU training

``` shell
# train p5 models
python train.py --workers 8 --device 0 --batch-size 32 --data data/data.yaml --img 640 640 --cfg cfg/training/JutePest-YOLO.yaml --weights '' --name JutePest-YOLO --hyp data/hyp.scratch.p5.yaml
```






## Citation

```
@ARTICLE{10535191,
  author={Zhang, Shuai and Wang, Heng and Zhang, Cong and Liu, Zheng and Jiang, Yiming and Yu, Lei},
  journal={IEEE Access}, 
  title={JutePest-YOLO: A Deep Learning Network for Jute Pest Identification and Detection}, 
  year={2024},
  volume={12},
  number={},
  pages={72938-72956},
  keywords={Feature extraction;Production;YOLO;Target recognition;Diseases;Crops;Computational modeling;Pest control;Deep learning;Jute pest detection;YOLOv7;PConv;wise-IoU;object detection;deep learning},
  doi={10.1109/ACCESS.2024.3403491}
}
```





## Acknowledgements

<details><summary> <b>Expand</b> </summary>

* [https://github.com/AlexeyAB/darknet](https://github.com/AlexeyAB/darknet)
* [https://github.com/WongKinYiu/yolor](https://github.com/WongKinYiu/yolor)
* [https://github.com/WongKinYiu/PyTorch_YOLOv4](https://github.com/WongKinYiu/PyTorch_YOLOv4)
* [https://github.com/WongKinYiu/ScaledYOLOv4](https://github.com/WongKinYiu/ScaledYOLOv4)
* [https://github.com/Megvii-BaseDetection/YOLOX](https://github.com/Megvii-BaseDetection/YOLOX)
* [https://github.com/ultralytics/yolov3](https://github.com/ultralytics/yolov3)
* [https://github.com/ultralytics/yolov5](https://github.com/ultralytics/yolov5)
* [https://github.com/DingXiaoH/RepVGG](https://github.com/DingXiaoH/RepVGG)
* [https://github.com/JUGGHM/OREPA_CVPR2022](https://github.com/JUGGHM/OREPA_CVPR2022)
* [https://github.com/TexasInstruments/edgeai-yolov5/tree/yolo-pose](https://github.com/TexasInstruments/edgeai-yolov5/tree/yolo-pose)

</details>
