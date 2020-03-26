# object_detection_colab
Train custom object detector in GPU-powered google colab 

This repository build upon EdjeElectronics' tutorial on training object detection for custom dataset using tensorflow API. Please follow the tutorial at https://github.com/EdjeElectronics/TensorFlow-Object-Detection-API-Tutorial-Train-Multiple-Objects-Windows-10.

Assuming you have followed the tutorial upto the "5b. Configure training" (just before the training part). Of course you can directly run the training on your PC/laptop, but this will run forever if you don't own any plausible GPU! Luckily, we can utilize the GPU available on publicly available Google Colab for the training.

Steps:
1. Clone this repository to your local directory on your PC/laptop. If you have done the tutorial upto "5b. Configure Training", you can skip this step and use your own folder instead.
2. Go to your google drive and paste the whole repository folder into the main google drive folder ("My Drive")
3. open ssdmobilenet-model-training.ipynb and run the cells. Don't forget to change the runtime to "GPU".
4. That's it. The training will start for multiple epochs.
5. The trained model.ckpt will be saved in the folder "training"
6. Finally, continue the tutorial in EdjeElectronics starting from "7. Export Inference Graph" and onwards.
