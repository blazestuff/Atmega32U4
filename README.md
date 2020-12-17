# Here is my project involving 
* an atmega32u4 (or similar)
* 2x pca9685 
* 24 servos
* wifi adaptor
* various sensors


The primary purpose of this project is to intergrate everything into a single board. This board will provide all necessary powerrails for every individual component, be it 3.3v, 5v,6v or even 12v. Such a feat would be simplier without the amperage hogs that are servos. The main supply power would likely be lithium batteries 18650. 4 in series would provide around 12v. But given my experience with 18650 cells, I will opt for something different. Sort of new, upcoming LiFePo4 or lithium iron phosphate. In terms of safety, they are infinitely more safe. So again I will use a 4s configuration. This is real overkill if not for the servos and would likely power the controller for months without needing a charge.

## pcb layout

The pcb layout will have to factor many things. Such as how noisy or how high (or low) the frequency will be. Do I need more than 1 cap for decoupling? Do I need an entirely isolated circuit for the massive draw of the servos compared to the other components?

* pretty much need to measure with a scope to see where the spikes/drops are at
* then need to decide on the decoupling configuration
* another mosfet for additional current?
* something along the lines of a TPS54386

Most of these questions have already been answered by myself, but I have yet to update a design. I like the boards that are usually paired with the atmega/tiny etc, but I wanted a fully custom design. One that fits my requirements exactly, that doesnt suffer unnecessary powerloss, board space, trace length and a gerber file that others could send off to the factory and replicate.
