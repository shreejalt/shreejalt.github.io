## Person Retrieval and Re-Identification

**Description:** Person Re-ID becomes a challenging task when there are lot of disturbances in the image such as occlusion, person-box aspect ratios, 
crop scales, and training the re-id models with present approaches of supervised classification and triplet matching when the number of classes are very high. Training the models on the public datasets like Duke-MTMC and Market1501 does not perform well on the issues mentioned as they are prominent in the real-world scenarios. I, therefore to tackle these problems, designed a Re-ID model which can take into consideration the box scale 
and alignment of a person crop for the best retrieval accuracy. I tested it on many datasets and I am mentioning the results on Market1501 using the proposed algorithm. Also, there was a 
significant gain observed when it was tested on the private company's datasets.


| Model                            | Data       | Rank@1 | Rank@5 | Rank@10 | mAP   |
| -------------------------------- | ---------- | ------ | ------ | ------- | ----- |
| Baseline                         | Market1501 | 94.63  | 98.25  | 99.05   | 85.24 |
| Baeline + Alignment + MultiScale | Market1501 | 96.59  | 98.84  | 99.44   | 91.24 |