## Site-Specific Training Tool

**Description:** When we want to scale the deep neural network such as object detector to many cameras and want to adapt with the specifics of the different
sites, we need good amount of label data to finetune the deployed model. To accomplish this, large amount of time is consumed for the data annotation process of different 
site specific data which can slow down the productivity of the deployed model. I designed and developed a proprietary light classifier architecture from scratch by incorporating the present and efficient in-house model backbones of the object detectors. It helped us to get around **8%mAP** improvements on a given site with very few amount of labeled images(~250-300). Also integrated
the BGS algorithm and introduced ***update-detect*** methodology with this tool which assisted in getting the seamless results on the low-FPS video streams of the surveillance cameras.

The given benchmarks are done on the private dataset of the company using the object detector(in-house). (LC: Lightweight Classifier / BGS: Background Subtraction Algorithm)

| Model                 | mAP  | P@0.5 | R@0.5 |
| --------------------- | ---- | ----- | ----- |
| Vanilla OD            | 64.9 | 87.9  | 54.8  |
| Vanilla OD + LC       | 72.5 | 88.3  | 62.9  |
| Vanilla OD + LC + BGS | 74.1 | 89.05 | 66.36 |