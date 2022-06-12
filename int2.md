## INT8 Quantization of Object Detectors

**Description:**  Quantization of object detectors by leveraging dynamic ReLU activation function for INT-8 calibration and
quantizing the weights of the model with the help of ***NVidia’s TensorRT’s algorithm(standalone implementation)*** . Dynamic ReLU viz. QReLU helped us to get only 0.5% drop after quantization and 1.2% increase in the overall mAP during training than the baseline.

### Design of the quantization process. 
<img src="/images/img1.png">

### Flowchart of INT8 Quantization
<img src="/images/img4.png">


