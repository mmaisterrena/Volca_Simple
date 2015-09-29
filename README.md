# Volca Simple
Use any midi keyboard to trigger samples in the Korg Volca Sample using an arduino as a midi channel re-router.<br>
Watch a demo video here: https://www.youtube.com/watch?v=zcMHnB5qIcQ

Developed by Mauricio Maisterrena.

# Requirements:

<strong>Hardware:</strong><br>
*Korg Volca Sample <br>
*Arduino Uno or Mega <br>
*Midi In:  <br>
   &nbsp;&nbsp;-Female MIDI jack Digikey CP-2350-ND <br>
   &nbsp;&nbsp;-220Ohm 1/4watt resistor Digikey CF14JT220RCT-ND <br>
   &nbsp;&nbsp;-1N4148 diode Digikey1N4148-TAPCT-ND <br>
   &nbsp;&nbsp;-10kOhm 1/4watt resistor Digikey CF14JT10K0CT-ND <br>
   &nbsp;&nbsp;-470 Ohm 1/4watt resistor Digikey CF14JT470RCT-ND (I used 2x220 instead) <br>
   &nbsp;&nbsp;-6N138 optocoupler Digikey 751-1263-5-ND <br>
 <br>
*Midi Out: <br>
   &nbsp;&nbsp;-Female MIDI jack <br>
   &nbsp;&nbsp;-220 ohm resistor <br>
   &nbsp;&nbsp;-Wires  <br>
   <br>
<strong>Software:</strong> <br>
 *Arduino MIDI library http://playground.arduino.cc/Main/MIDILibrary <br>


# Setup
* To recieve Midi messages with Arduino follow the next tutorial: http://www.instructables.com/id/Send-and-Receive-MIDI-with-Arduino/step10/Receive-MIDI-Messages-with-Arduino/
* To send Midi messages with Arduino follow the next tutorial: http://www.instructables.com/id/Send-and-Receive-MIDI-with-Arduino/#step1
* Install Arduino MIDI library http://playground.arduino.cc/Main/MIDILibrary
* Upload the Volca_Simple file to your Arduino. TIP: Make sure that Tx and Rx pins on the arduino are disconnected when uploading.
* Have Fun

# Usage
Connect any midi keyboard to the midi in on your arduino then connect the midi out of the arduino to the volca sample.
To trigger samples on the Volca Sample set your midi keyboard (or device) to midi channel 16 and play any note from C4 (midi note 60) to A4 (midi note 69). Each note will trigger a different sample.

# Donate

Help yourself by helping us support you! Many hours have been spent developing this code. Since you find it useful, please consider donating via the button below.

<a href=https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=C5GDLRY5Z4AXJ><img src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif" alt="PayPal - The safer, easier way to pay online!" /></a>
