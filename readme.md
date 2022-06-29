# yolor-a

# Install
```bash
$ git clone https://github.com/DijiesitelaQ/TSDetection
$ cd TSDetection
$ pip install -r requirements.txt
```

# Inference
* `Datasets` : [TT100k](http://cg.cs.tsinghua.edu.cn/traffic-sign/)
* `preweights` : [`yolor_p6.pt`](https://drive.google.com/file/d/1Tdn3yqpZ79X7R1Ql0zNlNScB1Dv9Fp76/view?usp=sharing)

$ python detect.py --source inference/images/ --cfg cfg/yolora_cbam.cfg --weights yolora_cbam.pt --conf 0.25 --img-size 1280 --device 0
# Train
train.py allows you to train new model from strach.
```bash
$ python train.py --batch-size 8 --img 1280 1280 --data coco.yaml --cfg cfg/yolora_cbam.cfg --weights '' --device 0  --hyp hyp.scratch.1280.yaml --epochs 300

```
```
```

# References
Thanks to their great works
* [yolor](https://github.com/WongKinYiu/yolor)

