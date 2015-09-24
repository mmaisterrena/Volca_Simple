# Volca Simple
Use any midi keyboard to trigger samples in the Korg Volca Sample using an arduino as a midi channel re-router.

# Requirements:

-Hardware:
*Korg Volca Sample
*Arduino Uno or Mega
*Midi In 
  *Female MIDI jack Digikey CP-2350-ND
  *220Ohm 1/4watt resistor Digikey CF14JT220RCT-ND
  *1N4148 diode Digikey1N4148-TAPCT-ND
  *10kOhm 1/4watt resistor Digikey CF14JT10K0CT-ND
  *470 Ohm 1/4watt resistor Digikey CF14JT470RCT-ND (I used 2x220 instead)
  *6N138 optocoupler Digikey 751-1263-5-ND
*Midi Out
  *Female MIDI jack
  *220 ohm resistor
  *Wires 
  
-Software
 *Arduino MIDI library http://playground.arduino.cc/Main/MIDILibrary


#Setup
* To recieve Midi messages with Arduino follow the next tutorial: http://www.instructables.com/id/Send-and-Receive-MIDI-with-Arduino/step10/Receive-MIDI-Messages-with-Arduino/
* To send Midi messages with Arduino follow the next tutorial: http://www.instructables.com/id/Send-and-Receive-MIDI-with-Arduino/#step1
* Install Arduino MIDI library http://playground.arduino.cc/Main/MIDILibrary
* Upload the Volca_Simple file to your Arduino
* Have Fun
