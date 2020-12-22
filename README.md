# Lithography-Hotspot-Detection

Lithography refers to the series of steps that establish the shapes, dimensions, and location of the various components of the integrated circuit. 

Lithography hotspot is a place where it is susceptible to open circuit or short circuit error due to poor printability of certain patterns in a design layout. 

To avoid undesirable patterns in layout, it is mandatory to find hotspots in the early design stage. 
Lithography simulation is computationally expensive way for hotspot detection so I chose Deep learning based technique and was able detect hotspots with an accuracy of 97.9%

It is based on following Research Paper: https://ieeexplore.ieee.org/document/8434561

Link for Dataset: http://appsrv.cse.cuhk.edu.hk/~hyyang/files/iccad-official.tgz

More Details about Dataset: https://appsrv.cse.cuhk.edu.hk/~hyyang/files/hsd-web/index.html

Dataset used for implementation:
Dataset used is ICCAD benchmark dataset and data is unlabelled. It has five sub-datasets:
ICCAD_1: It consists of 440 training images(100 with hotspot and 340 without hotspot) and  4907 testing images(227 with hotspot and 4680 without hotspot)
ICCAD_2: It consists of 5401 training images(175 with hotspot and 5226 without hotspot) and  testing images 41,798 (499 with hotspot and 41,299 without hotspot)
ICCAD_3: It consists of training images 5,554 (with 910 hotspot and 4644 without hotspot) and  testing images 48,143 (1809 with hotspot and 46334 without hotspot)
ICCAD_4: It consists of training images 4549 (96 with hotspot and 4453 without hotspot) and  32069 testing images(178 with hotspot and 31891 without hotspot)
ICCAD_5: It consists of training images 2744 (27 with hotspot and 2717 without hotspot) and  testing images 19370 (42 with hotspot and 19328 without hotspot)

Hyper-Parameters Used:

Epochs use <= 20

Model = Sequential
Layers                                                                                   Hyper-parameters
Multilayer Perceptron                                  Layers = 8,Batch Size = 64, Image Shape = 224,224,3
CNN                                                             Filters = 12, Kernel size = (3,3), activation = ELU
CNN                                                             Filters = 12, Kernel size = (3,3), activation = ELU
CNN                                                             Filters = 12, Kernel size = (3,3), activation = None
Batch Normalization                                    momentum=0.99, epsilon=0.001
Activation                                                     type = ELU
MaxPooling                                                  pooling window = (2,2)
