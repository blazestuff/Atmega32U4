# here is my project involving 
* an atmega32u4 (or similar)
* 2x pca9685 
* 24 servos
* wifi adaptor
* various sensors


The primary purpose of this project is to intergrate everything into a single board. This board will provide all necessary powerrails for every individual component, be it 3.3v, 5v,6v or even 12v. Such a feat would be simplier without the amperage hogs that are servos. The main supply power would likely be lithium batteries 18650. 4 in series would provide around 12v. But given my experience with 18650 cells, I will opt for something different. Sort of new, upcoming LiFePo4 or lithium iron phosphate. In terms of safety, they are infinitely more safe. So again I will use a 4s configuration. This is real overkill if not for the servos and would likely power the controller for months without needing a charge.

