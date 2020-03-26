# object_detection_colab
Train custom object detector in GPU-powered google colab 

This repository builds upon EdjeElectronics' tutorial on training object detection for custom dataset using tensorflow API. Please follow the tutorial at https://github.com/EdjeElectronics/TensorFlow-Object-Detection-API-Tutorial-Train-Multiple-Objects-Windows-10.

Assuming you have followed the tutorial upto the "5b. Configure training" (just before the training part). Of course you can directly run the training on your PC/laptop, but this will run forever if you don't own any plausible GPU! Luckily, we can utilize the GPU available on publicly available Google Colab for the training.

Steps:
1. If you have done the tutorial upto "5b. Configure Training", you should already have a folder named "model" downloaded from https://github.com/tensorflow/models. You may create a folder named "object_detection_train" and dump the "model" folder inside".
2. Go to your google drive and paste the whole "object_detection_train" folder into the main google drive folder ("My Drive")
3. Download "ssdmobilenet-model-training.ipynb" and upload to your google drive as well, inside the "object_detection_train" folder.
4. Download "ssd_mobilenet_v2_coco.config" file and paste it in the "object_detection_train\models\research\object_detection\training" folder in your gdrive.
5. open ssdmobilenet-model-training.ipynb and run the cells. Don't forget to change the runtime to "GPU".
6. That's it. The training will start for multiple epochs.
7. The trained model.ckpt will be saved in the folder "training" or any folder you want to.
8. Finally, continue the tutorial in EdjeElectronics starting from "7. Export Inference Graph" and onwards.
