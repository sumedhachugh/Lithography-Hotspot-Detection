# Lithography-Hotspot-Detection

Lithography technique is used to pattern specific shapes of a thin layer on a rigid substrate for fabricating electrical devices.

Lithography hotspot is a place where it is susceptible to open circuit or short circuit error due to poor printability of certain patterns in a design layout. 

To avoid undesirable patterns in layout, it is mandatory to find hotspots in the early design stage. 
Lithography simulation is computationally expensive way for hotspot detection so I chose Deep learning based technique and was able detect hotspots with an accuracy of 97.9%

## Folder titled 'notebooks' contains code files 

Link for Dataset: http://appsrv.cse.cuhk.edu.hk/~hyyang/files/iccad-official.tgz

More Details about Dataset: https://appsrv.cse.cuhk.edu.hk/~hyyang/files/hsd-web/index.html

Dataset used for implementation:
Dataset used is ICCAD benchmark dataset. It has five sub-datasets:

Sub-Daaset_1: It consists of 440 training images(100 with hotspot and 340 without hotspot) and  4907 testing images(227 with hotspot and 4680 without hotspot)

Sub-Daaset_2: It consists of 5401 training images(175 with hotspot and 5226 without hotspot) and  testing images 41,798 (499 with hotspot and 41,299 without hotspot)

Sub-Daaset_3: It consists of training images 5,554 (with 910 hotspot and 4644 without hotspot) and  testing images 48,143 (1809 with hotspot and 46334 without hotspot)

Sub-Daaset_4: It consists of training images 4549 (96 with hotspot and 4453 without hotspot) and  32069 testing images(178 with hotspot and 31891 without hotspot)

Sub-Daaset_5: It consists of training images 2744 (27 with hotspot and 2717 without hotspot) and  testing images 19370 (42 with hotspot and 19328 without hotspot)


