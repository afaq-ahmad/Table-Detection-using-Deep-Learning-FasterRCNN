# Table-Detection-using-Deep-Learning-on-Google-Colab
Table Detection using Deep Learning in a pdf.

Table detection part is followed by this paper
[Table Detection using Deep Learning](https://tukl.seecs.nust.edu.pk/members/projects/conference/Table-Detection-Using-Deep-Learning.pdf)
, kindly site it if you are using it.



#### Image_preprocessing:
    min_size: 600
    max_size: 1024

#### Data_augmentation:
    - flip:
        left_right: True
        up_down: True
        prob: 0.5
#### Model:
    type: fasterrcnn
    network:
      # Total number of classes to predict.
      num_classes: 1

### Procedure:
>Training:
    
    - Run the code "1_Table_Detection_Training.ipynb" on colab python 3
    - Upload the data.zip in colab directory
    - Save the model(checkpoint) .tar File in google drive for Testing Purpose.

>Testing:
    
    - Run the code "2_Table_Detection_Testing.ipynb" in colab python 3
    - Import the model(checkpoint) from google Drive **use same name of checkpoint**/
    - Upload the "test_sample.png" image for testing from image.
    - For testing From Pdf first run the code "Pdf_To_images.ipynb" in local directory <it will save the pdf to jpg images>
    - Upload the zip of images on colab and run the next section pDF table detection
    - The end product will be saved as Pdf file check the file for accuracy of given model detector.
  
  
 
