<h1><center>CIFAR-10 Dataset</center></h1>

Many different models have been tested applying different sets of techniques in order to improve accuracy on CIFAR-10 Dataset.
 


| <div style="text-align: center"> Model  </div>| Accuracy (%)|Loss|# Parameters| # Dense layers |# Convol. layers|Reg. Type|
| ------------- | ------------- |------------- | ------------- |------------- | ------------- |------------- |
|  <div style="text-align: left"> 1. Single-Layer Perceptron </div>|<center>40.12</center> | 1.7347</center> |30,730 |1 |- |<center> No</center> |
| <div style="text-align: left"> 2. Multi-Layer Perceptron </div>||||| ||
| <div style="text-align: left"> <ul>2.1. Fully connected layers</ul> </div>|<center>47.38</center>|1.4854</center> |1,313,710 |4 |- |<center> No</center>|
| <div style="text-align: left"><ul> 2.2. Switched to Leaky ReLU </ul> </div>|<center>51.72</center>|1.4213</center> |1,313,710 |4|- |<center> No</center>|
| <div style="text-align: left"> <ul>2.3. Added more layers </ul></div>|<center>49.77</center>|    <center>1.4359</center> |1,394,210 |6 |- |<center> No</center> |
| <div style="text-align: left"> <ul>2.4. With regularization </ul></div>|<center>46.70</center>    |<center>1.9480</center> |1,331,910 |4 |- |<center> Batch Normalization</center> |
| <div style="text-align: left"> <ul>2.5. With regularization </ul></div> |<center>54.11</center> | <center>1.3409</center> |1,313,710 |4 |- |<center> Data Augmentation</center> |
| <div style="text-align: left"> 3. Convolutional Neural Network </div>|    | | | | ||
| <div style="text-align: left"> <ul>3.1. Multi-layer convolutional neural network </ul> </div>|  <center>69.61</center>    |<center>2.0431</center> |936,010 |2 |2 |<center> No</center>|
| <div style="text-align: left"> <ul> 3.2. Added more layers</ul></div>   |  <center>72.83</center>    |<center>1.5127</center>|225,034 |2 |3 |<center> No</center> |
| <div style="text-align: left"> <ul> 3.2. With regularization </ul></div>   |  <center>75.01</center>   |<center>0.7725</center>|225,034 |2 |3 |<center> Early stopping</center> |
| <div style="text-align: left"> <ul> 3.3. With increased regularization </ul></div>   |  <center>74.78</center>    |<center>0.7469</center>|225,034 |2 |3 |<center> Early stopping & Dropout</center> |
| <div style="text-align: left"> <ul>3.4.'LeNet-5' type with regularization  </ul></div>   | <center>52.40</center>    |<center>1.5309</center>|121,182 |3 |2 |<center> Weight decay (L2)</center> |
| <div style="text-align: left"> <ul> 3.5. With mean std. normalization </ul></div>   | <center>73.92</center>|1.5885</center>|225,034 |2 |3 |<center> No</center> |
| <div style="text-align: left"> <ul> 3.6. Added regularization </ul></div>   |  <center>75.62</center>    |<center>0.8183</center>|225,034 |2 |3 |<center> Early stopping</center> |
| <div style="text-align: left"><ul> 3.7.'Network in Network' with mean std. normalization </ul></div>   |  <center>80.19</center>    |<center>0.8769</center>|972,658 |0 |9 |<center> Early stopping, Dropout <br>Batch Norm. & Data Augmentation</center> |
| <div style="text-align: left"><ul> 3.8.'VGG-16' architecture with mean std. normalization  </ul></div>   |  <center>81.34</center>    |<center>1.0168</center>|15,001,418 |2 |13 |<center> Early stopping, Dropout <br>Batch Norm. & Data Augmentation</center> |
| <div style="text-align: left"><ul> 3.9.'VGG-16' architecture with mean std. normalization  </ul></div>   |  <center>87.86</center>    |<center>0.9219 </center>|15,001,418|2 |13 |<center> Early stopping, Dropout <br>Batch Norm. & Data Augmentation</center> |



**NOTES:** 
1. All convolutional layers are followed by a Pooling layer (max pooling). 
2. All models have been trained with *batch size*=128.
3. LeNet, VGG-16 and Network in Network architecture's credit goes to their authors (mentioned below).
