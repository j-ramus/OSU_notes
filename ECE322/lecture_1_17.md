## CLamping circuits

limits peaks of input waves

AKA clipping circuit

applicatons: protecitng input gate of mosfets or other devices

example: diode with 0.7v $V_B$ and ouptut is taken across diode. 
if the inputis 0.5v there is no voltage drop, and the output is still 0.5v

if input voltage goes to 0.8v, the diode will still be 0.7
The voltage drop across the resistor before the didode bercause 

if input is -1v, the output will also be -1v

reversing anode/cathode clamps at -0.7v

doiodes can be put in series for higher clamping limit

if power supply on other side of diode, vout is 0.7 + that supply

it must overcome the reverse poer supply and the voltage drop. Once that is overcome, and voltage above 0.7 
upply goes to ground.

## DC restoration

square wave -5v to 5v

we want to shift to 0v to 10v

supply -> capacitor -> output node -> diode cathode -> ground

if -5 at $\tao=0$ both sides of capactior are -5v



shotsky diodes have lower $V_B$

sssss diodes do 2way clamping. main application gives reference voltage

