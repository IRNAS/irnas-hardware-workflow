# Development-prototype board design tips

Resons for making Development-prototype board when starting new project are:
* Firmware development can start sooner - this is probably the most important since FW typically takes an order of magnitude longer than HW design
* Verify PCB footprints for components
* Power Measurement
* Helps you get a feel for how small you can make the design once everything is working.

Here are the a few tips for how to design development/prototype boards:
* Expose all the pins of the components on test points or at least SMT pads.
* Include a serial port (UART header).
* Related to the above, bring out all signals that you can on easy 0.100" headers. You can then attach logic analyzers, scopes, etc. Label them all with their signal name.
* Label liberally. Silkscreen is free, so on a development board label all components, as well as the signals on 0.100 headers, etc.
* If it is a RF design with an onboard antenna, make an option for a connector. Can be SMA, U.FL or whatever, but something that you can connect to directly.
* Include a power connector, easier for firmware dewelopment.
* Enable power measurement: add a 0.100" header between LDO output and power input. This will have a shunt that can be removed and an ammeter attached instead. For extra credit, do this for the major power subsystems of the circuit.
* Use full-sized JTAG connectors, and used shrouded (polarized) headers to prevent having to think about it.

To see the original text go to [link](http://fixituntilitsbroken.blogspot.rs/2011/03/making-development-boards-that-dont.html)
