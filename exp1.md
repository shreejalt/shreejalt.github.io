## Redifining One-Shot Object Detector For Two Class Problem

**Description:** One shot object detectors face the anchor problems when the dataset is biased and high variance in the box sizes. To tackle that issue, I developed a hierarchial clustering approach to adjust the anchors height and width viz. **Anchor Search** algorithm for assigning and learning optimal anchors for two different classes individually. This was developed by taking into consideration the two classes i.e person ***body*** and ***head*** which somewhat vary a lot in the size and aspect ratio. Also entangled the training of head and body of person together instead of treating them as two different classes 3% mAP gains were observed after final bench-marking the improvements.

### Results on the final improvements.

| Detector Model                                       | AP Head | AP Body   |
| ---------------------------------------------------- | ------- | --------- |
| In-house Vanilla Detector                            | 88.5%   | 87.5%     |
| In-house Vanilla Detector + Anchor Search            | 90.02%  | 90.11%    |
| In-house Vanilla Detector + Anchor Search + Entangle | **91%** | **91.9%** |
