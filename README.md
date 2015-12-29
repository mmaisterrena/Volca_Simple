# Volca Simple
Makes it posible to play pitched notes on the Volca Sample using a midi keyboard by sending different speed values when playing notes. also enables you to trigger any sample using just one midi channel.

Developed by Mauricio Maisterrena (December 2015, Torreon Coah. Mexico).

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

1. Trigger samples using just 1 midi channel: Set your midi keyboard (or device) to midi channel 16 and play any note from midi note 0 (the lowest possible note) to midi note 9. Each note will trigger a different sample.

2. Trigger pithched notes using a keyboard (monophonic): Set your midi keyboard to any midi channel between 1 and 10 (each channel will trigger a different sample) and play notes from midi note 36 (C2) to midi note 84 (C6).

3. 4 Voice Polyphonic Synth: Set the last 4 samples in your Volca Sample (samples 7 to 10) to the same pitched sample, set your midi keyboard to midi channel 16 and play notes from midi note 36 (C2) to midi note 84 (C6).

*Recomended: For better results when playing pitched notes always use samples tuned to midi note 60 (C4) as the "seed" sample.


# Donate

Help yourself by helping us support you! Many hours have been spent developing this code. Since you find it useful, please consider donating via the button below.

<a href=https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=C5GDLRY5Z4AXJ><img src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif" alt="PayPal - The safer, easier way to pay online!" /></a>
