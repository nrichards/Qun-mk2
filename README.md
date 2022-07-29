#### ** Please send email to info@nunomo.net , or open issues for inquiries. **


# Qun-mk2

Qun-mk2 is a small synthesizer with powerful sound engine, sequencer and looper.

![qun_mk2_cgi](./manual_images/qun_mk2_cgi.png)

## Links and Information

* [Online Shop](https://shop.nunomo.net/products/): Purchase your own one from our website.
* [Presets](https://github.com/raspy135/Qun-mk2/blob/main/sd_template.zip) for tone presets. We constantly update the tone presets.
* [Issues](https://github.com/raspy135/Qun-synthesizer/issues): Report issues when you have problems or questions.
* [Firmware](./firmware): For firmware updates.
* [CheetSheet](./cheetsheet.pdf) : For cheet sheet.

**We are looking for your feedback! For general impressions and feedback, please email them to info@nunomo.net.**

## Overview of the QUN mk2
Qun mk2 has two-oscillator virtual analog, FM, granular sound engine. 2 oscillators can be used separately.

A sequencer is 8-step based sequencer, supports up to 32/64 steps. You can store 8 patterns for each preset. It has 8 preset and sequencer pattern buckets. You can switch 8 presets and 64 patterns quickly.

Three track looper with 5 scenes, you can swap 3 track x 5 scenes while playing. 

* **Analog Modeling engine**
  * The analog modeling engine is **an original, made from scratch**. It uses advanced algorithms for great organic sound. The engine is not a copy of a classic synth, it is designed to make modern sounds.
  * Low latency.
  * All analog modeling engine parameters can be configured through MIDI. 
  * Clean 2 Oscillators. Cheap synthesizers compromise this part sometimes, but QUN has no-alias noise Oscillators. All of the internal calculation is done by floating point for the sound quality.
  * Oscillators can be used as 1 oscillator per voice, or 2 oscillators per voice.
  * Voice can be configured as 4 voices (Quad mode) or 2 voices (Dual mono).
  * The sound engine is compatible with Qun mk1. 
  * Multiple QUN synths can be stacked to achieve a **Polyphonic** setup. 
  * **Flexible MOD (CV) routing**. 
  * 2 inputs can be used for **external audio signal**, or **external CV inputs**
  * 4 Envelope Generators
  * FM (4 Operators x 2)
  * **Granular / Sampler engine**
  * 1 LFO, rate can be controlled by MIDI notes
  * 1 Organic sounding VCF
    * 2/4 Poles, Low-pass, Band-pass, High-pass, Notch)
    * Key sync
  * 1 Effect (Delay, Chorus, Flanger, BitCrusher)
  * MIDI clock sync
* Player / Sequencer
  * Player (piano mode)
  * MIDI out to control external synths
  * **8/16 step sequencer has 4 pages, up to 64-step sequencer** will generate inspiring beats for you
    * Note On/Off/Double/Triple
    * Transpose / Note width (Length) / Velocity / Probability
    * Randomness
    * Scale quantize
    * Arpeggiate steps
    * Shuffle
  * Looper
    * Sequencer synchronized, internal or externally clocked.
    * Looper can record the sound up to around 30 sec for each recording.
    * You can record the sound from sound engine or external audio.
    * **3 tracks**, **5 Scenes**, total 15 recordings in one Session
    * Scene change while playing (Something like Ableton Live's session view)
    * Cut / Paste
    * Play / Rec / Overdub
  * Mixer
  	* Looper tracks can be panned for stereo
  	* Integrated compressor (Fixed parameters: 30ms attack, 100ms release, 1:3)
  	* Stereo output
  	* Mute by track
  * Micro SD card
  	* Qun mk2 comes with micro SD card.
  	* All looper recordings, preset and granular sample is stored to SD card

## QUICK START

https://www.youtube.com/watch?v=yVATR95V4To

is the good video to get started.

Factory presets are installed in bank 7 and bank 8. You can always download the presets from this site, under preset folder, or download sd_template.zip.

## CONNECTIONS

* Power: Use a good quality USB power supply. Connect the USB cable to `POWER` labeled USB port (Top one).
* MIDI: Use **TRS A** MIDI adapter to connect MIDI cables. TRS A type adapter is the same as KORG, AKAI and Make Noise's adapter. This is the lowest latency option. The synth comes with MIDI TRS A cable.
* It has microphones and stereo line input.
* LINE IN and PHONE OUT is located at right side. Output is not strong, so please connect to headphone amp or mixer. Looper mixer is stereo. **Please use a stereo cable for the sound input and output**. 
* It comes with micro SD card. Qun mk2 always needs SD card. SDHC is supported. Class 10 card (Normally it's indicated as Circled 10) or higher is required to satisfy the bandwidth. It's safe to remove when the access indicater is not lid, but it's not hot swappable, Please reset the device when you remove SD card.

## MAJOR MODES

 The synth has three major modes. 

Button | Function
------------ | -------------
Play | Play Mode. It’s for sequencer / looper. 
System | Setting. For load / save / system setting.
Param | Parameter Mode. Change synthesizer’s parameters.

## BASIC OPERATION

Each major mode has sub modes. Select sub mode. For example, `OSC1` is a sub mode for Oscillator 1.

* To switch sub mode, press SHIFT button + rotate dial. Keep pressing Mode button while you are selecting sub mode.
* Alternatively, you can press SHIFT + 1-8 button or NO/OK buttons to change sub mode.

After you enter the sub mode you want, press 1-8 button to select parameter.
* Press one of 8 buttons + rotate dial = Change parameter
* Rotate the dial = Change the current parameter.
* If you want to do fine value adjustment, you can use NO/OK buttons to change the value by 1. To do this, keep pressing one of 8 buttons and press NO or OK button.
* Once you entered the adjustment mode, dial is disabled while you keep pressing one of 8 buttons. However, it can be used as "Catch" mode. When the current value is matched with the knob value, "*" is indicated next to value. You can use this feature to avoid value jumping.

Button | Primary function
------------ | -------------
SHIFT | Shift + [1-8] button or NO/OK button to select sub mode 
[1-8] button | Select parameter in selected sub mode
NO | Select previous sequencer pattern
OK | Select next sequencer pattern
Dial | change parameters
SEQ PLAY | Start / Stop sequencer
MODE PLAY | Select Play mode
SYSTEM | Select System mode
PARAM | Select Param mode
LOOPER REC + LOOPER PLAY | Start looper recording
LOOPER PLAY | Start looper playing
LOOPER STOP | Stop looper playing
RST button on the base board | Reset the device

## BASIC SHORTCUTS

Button | Function
------------ | -------------
SHIFT + MODE PLAY | Dumping current preset to MIDI OUT. This is useful to transfer current preset to another Qun / Qun mk2 synthesizer.
SHIFT + SYSTEM | All notes off
SHIFT + PARAM | Initialize the preset
SHIFT + SEQ PLAY + turn dial | Set BPM
MODE PLAY + turn dial | Record volume
SYSTEM + turn dial | VCF volume
PARAM + turn dial | VCF cutoff
REC + turn dial | LFO tune
LOOPER PLAY + [1-5] | Select Scene
REC + [1-3] | Select Track
PARAM + [1-3] | Mute track
MODE PLAY + [1-8] | Recall preset bucket
SEQ PLAY + [1-8] | Select Sequencer pattern
SHIFT + LOOPER PLAY + turn dial | Load session when you are not in System mode or Granular mode. 
SHIFT + LOOPER PLAY + [1-3] button | Import wav file from import folder to selected track

## LED indicators

![leds](./manual_images/leds.png)

The synth has 8 LED indicators on the switch.
Solid LED shows selected pattern number.

- When playing, another LED shows current position of the sequencer.
- When trying to switch Scene (When pressing LOOPER PLAY) shows current selected Scene.
- When trying to switch Track (When pressing LOOPER REC) shows current selected Track
- When trying to mute Track (When pressing PARAM) shows current mute status of the Tracks.
- When trying to switch bucket (When pressing MODE PLAY) shows current selected Bucket.


## MIDI learning

Assigning proper MIDI CC to your MIDI keyboard is recommended for frequently used parameters, however, you can override MIDI CC temporary by the following operation:

1. In parameter mode, press corresponding MIDI CC button long time (about 3 sec). For example, OSC1's Pulse Width is button 2 in OSC1 sub mode.
2. Then "MIDI Learning" message is shown. Keep pressing the button.
3. Send MIDI CC signal from your MIDI keyboard (Turn the knob or move fader). The sent MIDI CC# will control the assigned parameter.

Once the parameter is assigned, then "*" mark is indicated before the CC number. Original CC assignment is still working. It won't be affected with MIDI dumping.
MIDI learning will take any MIDI channel. For example, even if you set the device to receive MIDI channel 2, MIDI learning can receive CC# for channel 3, or any other channels.

To cancel the override, do the same operation again.

To avoid confusion, this setting won't be saved.

## Session


![data_structure](./manual_images/data_structure.002.png)

Session is the biggest data unit of the synth.
Session includes 8 preset buckets. Each bucket contains one preset with 8 pattern sequencer data.
Looper recording (5 Scenes * 3 tracks) and Mixer data will be saved in the session.
Saving session is performed half-automatically. Looper recording data will be saved immediately after the recording. 
Mixer and Bucket data will be saved quietly when looper is stopped. You can manually execute it by pressing LOOPER STOP button.

There is no "new session" function. The synth always create a new session when booting.

To load session, press SHIFT + LOOPER PLAY when you are not in System mode or Granular mode. Current session number "Session:0001" will be indicated. Turn dial to select the session you want to load.

If you want to load older than recent 32 session, you can press NO / OK button to scroll the page.

You can import WAV files to session. Put WAV files under "import" folder. Folder structure is supported so you can make subfolders to organize samples.
WAV format has to be **16-bit, 48000Hz, Mono**. Otherwise "Format error" message is shown.

To import file, set proper BPM first, then press SHIFT + LOOPER PLAY + [1-3] button. [1-3] button corresponds the destination track.
The data is trimmed to the closest the end of the measure.

If you have existing recordings in the session, WAV file will be cut to the current scene's looper length. You can use empty recorded track just to cut the WAV file to match the loop length. Otherwise it's trimmed to the longest point of the end of the measure.

## Preset bucket

The synth has 8 preset buckets to recall preset quickly. This is powerful feature with looper.

![data_structure](./manual_images/data_structure.001.png)

Bucket information is automatically saved with Session when looper is stopped. 

Each bucket contains one preset and 8 sequencer pattern.
In order to switch between bucket, press MODE PLAY + [1-8] buttons.
Solid LED indicates current bucket you are in when pressing MODE PLAY button.

To understand how bucket works, try the following steps:

1. Reset the board
2. Change some parameter to configure the sound, let's set it to Sine wave.
3. Press Recall(Mode/Play) + Button 2 to switch Bucket 2
4. Then the sound should be changed to the default SAW wave.
5. Change some parameters to program, let's set it to White noise.
5. Press Recall + Button 1 to switch back to Bucket 1
6. The first sound you configured should be recalled.
7. Press Recall + Button 2 to switch to Bucket 2 again
8. White noise should be recalled.

There is no copy function between bucket, but you can use preset bank 1 to bank 8 as a copy buffer.
When you save the preset or load the preset from bank 1 to 8, the name is used to indicate the bucket, so always recommending to set name by saving or loding preset.

Bucket doesn't contain Granular's sample data, however, bucket tries to find a sample from preset folder when the bucket has a name. So if you save the tone preset in bank1 to bank8, Granular's sample will be loaded automatically when the bucket is selected.


## Signal diagram

![qun2_signal_diagram](./manual_images/qun2_signal_diagram.png)

## Parameter Mode

### PRM:OSCILLATOR1,2
This diagram shows OSC1 and OSC2 features. The diagram is for explanation, it may not cover all features in the OSCs. All parameters can be controlled via MIDI including dials.

**Blue: Sources | Green: Output**
![diagram_osc](manual_images/diagram_osc.jpg)

The oscillator is a hybrid of classic analog synth and FM. FM has its own parameters, it can be configured in FM conf / ENV3/4 Other Mode.

The QUN's CV input routing is very flexible. One CV is connected to LFO (for tune/width), another one is selectable. It could be one of EG1 to EG4, AUX (Audio in), OSC2 signal, OSC2 signal after EG processing, Freq level out from OSC1, or Freq level out from OSC2.

1. SHAPE

	`Saw, Sine, S&H, Square, Triangle, W Noise, P Noise, FM, AUX`
	*AUX means audio input from LINE or MIC.
	*FM has 4 operators inside. See FM Conf Sub mode for detail.
	*Granular synth engine can be connected to AUX L channel. See Granular sub mode for detail.

2. PULSE WIDTH
	
	The synth has an unique behavior with pulse width.
	You can modulate the wave shape by pulse width, not only limited to Square wave.
	
	* Triangle
	* SAW
* Square
	
3. TUNE

4. OCTAVE

5. MOD TUNE

	MOD bus feedback to tune.

6. MOD WIDTH

	MOD bus feedback to pulse width.

7. LFO TUNE

	LFO feedback to tune.

8. LFO WIDTH

	LFO feedback to pulse width.

### PRM:MIX
Mix controls mixer and effects.

![diagram_mix_aux](manual_images/diagram_mix_aux.jpg)

1. OSC MIX

	Balance between OSC1 and OSC2

2. FM

	FM modulation OSC2 to OSC1. 
	That means that each oscillator has internal 4 operator FM, on top of it, you can modulate OSC1 by OSC2.

3. VCF VOLUME

	Volume to VCF. It can be used as generic volume control.

4. AUDIO IN GAIN

	GAIN from Line in / Mic In

![diagram_effector](manual_images/diagram_effector.jpg)

5. EFFECT TYPE

  Off, Delay, Chorus1, Chorus2, Flanger1, Flanger2, Crusher (Bit crusher), MDelay(Mono delay), RSVD(Reserved for the future update)

6. EFFECT SPEED

	Controls Effect LFO rate or delay time

7. EFFECT DEPTH

	Amount of effect

8. EFFECT FEEDBACK

	Feedback for Delay

#### Effector tips
- Effector became stereo since the firmware v3.30
- The Delay speed can be set very short. Very short delay can be used to create an interesting simulation of flute or violin. Mono Delay will work better for the use delay as a resonator.
- You can widen stereo image by short delay. 
  - Effector Type : Delay
  - Speed : Around 30
  - Depth : Around 30
  - Feedback : 0

### PRM:ENV1/2
The synth has four Envelope generators. ENV1 and ENV2 are both independently and fully configurable. ENV3 and ENV4 shares the parameter. Also ENV3 / ENV4 is connected to FM operators.
ENV1 and ENV2 are grouped to first voice with Quad mode. ENV3 and ENV4 are grouped to second voice with Quad mode.

![diagram_eg](manual_images/diagram_eg.jpg)

1/5 . ATTACK

	Attack time

2/6 . DECAY

	Decay time

3/7 . SUSTAIN

	Sustain level

4/8 . RELEASE

	Release time

### PRM:OSC Switches
OSC has many switches to change its behavior.

1/5 . ENV Sel

	Selects Envelope(VCA) for the oscillator.
	`EG1, EG2, EG3, EG4, AUX, OSC2, OSC2EG, FRQ1, FRQ2, ON`
2/6 . WIDE TUNE

	When it is ON, you can tune wider range by OSC’s tune parameter.
3/7 . MOD SEL

	Select Mod signal source. It is connected to OSC's tune or width.
	`EG1, EG2, EG3, EG4, AUX, OSC2, OSC2EG, FRQ1, FRQ2, ON`

4/8 . ENV INV SW

	It inverts Envelope Generator’s polarity. ENV1 and ENV2 can change its polarity.

### PRM:LFO
LFO is similar to OSC, although selectable shape is slightly different.

External clock sync setting is available in "PRM:KEY/OTHER" menu.

![diagram_lfo](manual_images/diagram_lfo.jpg)

1. LFO TUNE

	Tune

2. LFO SHAPE

	`Saw, Sine, RevSaw, S&H, Square, Triangle, AUX, OSC2, OSC2EG`
	*AUX is audio input from LINE / MIC.
	*You can use OSC2 as LFO source. You can even modulate OSC2 with OSC2.
	*OSC2EG is the signal from OSC after Envelope Generator processing.

3. LFO PULSE WIDTH

	Pulse width

4. LFO MOD TUNE

	Envelope generator feedback to tune.

5. LFO MOD WIDTH

	Envelope generator feedback to pulse width.

6. KEYSPLIT

	This is a unique feature of the synth.
	When it is not zero, then note number above the parameter becomes LFO rate controller. If you set 60, then C4 or higher note becomes LFO controller.
	Higher notes will generate higher LFO rate.
	If you press multiple notes, it doubles and triples the rate, great for live performance.

7. LFO GATESYNC

	LFO’s phase is reset by every note hit when it is ON.

8. LFO MOD SEL

	`EG1, EG2, EG3, EG4, AUX, OSC2, OSC2EG, FRQ1, FRQ2`

### PRM:VCF
The synth has one filter. LPF / BPF/ HPF / Notch can be selected. It also has a 4/2 poles switch, and linear and non-linear switch. Linear gives organic resonance, Non-linear gives more character.

![diagram_vcf](manual_images/diagram_vcf.jpg)

1. CUTOFF

	Set the cutoff frequency.

2. RESONANCE

	Resonance.

3. VCF TYPE

	`LPF,BPF,HPF,Notch`.

4. VCF MOD CUTOFF

	Mod feedback to cutoff. Mod source selection is located in `Prm:Key / Other` sub mode.

5. VCF LFO CUTOFF

	LFO to cutoff feedback.

6. VCF LFO Volume

	LFO feedback to VCF’s input volume.

7. OSC1 Bypass

  OSC1 can skip VCF. HALF means 1st half of 4-pole filter.

8. VCF KEY SYNC

	When it is not zero, VCF’s cutoff will follows the playing note. Higher value is more sensitive.
	Great with Mono, but not working well with Quad tone because it has only one VCF.

### PRM:KEY/OTHER
Configures other parameters.

1. VCF 4/2 POLE / NoLinear

	Change filter's number of poles, and selects linear or non-linear. 2 Poles is -12db/oct, 4 Poles is -24db/oct. 2 Poles filter gives brighter character. Linear(LI) has less character, but linear's resonance is sharp and more organic like real instruments. Non-linear(NL) has more character, has more harmonics, close to other synthesizers. 
	If you use cutoff envelope or copying patch from other synths, typically Non-linear is suitable.
	If you are trying to achieve something close to a real instrument or you want clear sound, linear is suitable.

2. VCF MOD SEL

	`EG1, EG2, EG3, EG4, AUX, OSC2, OSC2EG, FRQ1, FRQ2, ON`.

3. GLIDE

	Tune changes gradient when the value is not zero. Works with Mono.

4. BEND RANGE

	Pitch bend range.

5. OSC1/2 Keysync

	This is a switch to connect MIDI input note and oscillators. Y = Follow MIDI note pitch. N =Ignore MIDI note pitch. This is useful when you make percussion sound.
    You can still use freq1 freq2 for modulation to use MIDI note pitch.

6. VELOCITY SW

	Envelope generators become velocity sensitive when it’s ON.

7. MONO/QUAD/POLY (Voice mode)

  One synthesizer can be used as Monophonic or Quadphonic.

  * Mono = Mono (2 OSCs per voice)
  * Quad = Quad Tone (1 OSC per voice, and the engine has total 4 oscillators for the extra voices)
  * PolyMono = 2 OSCs per voice, but you can get 2 voices

  When the mode is Quad or Poly Quad, MIX  and "OSC2 Env Sel" are ignored. MIX is always set to middle, and OSC2 Env Sel is always set to EG2.
   Most of cases you want to use the same parameters between Osc1 and Osc2 with Quad mode. 

  To copy the parameter from OSC1 to OSC2 (and EG1 and EG2), long press button 7. "OSCs synched" message will be shown. 

  Here is an example to set up Quad mode
  1. Initialize tone.
   2. Configure OSC1 as you like.
  3. Set this parameter to "Quad" mode by pressing button 7.
   4. If you want to copy OSC1 parameters to OSC2, in the same submode, long press button 7 until "OSCs synched" message shown.
  5. Play two notes by external MIDI keyboard. You will hear four voices.

   Poly Mono can be used when you want 2 voices with 2Oscs per voice configuration.

   Poly Quad is for multiple device stacked configuration. You can use multiple Qun Synthesizers to build polyphonic synth.
  Please see “Polyphonic setup” for detail.

8. LFO SYNC SW

	LFO rate will synchronize with MIDI clock when it is ON.

### PRM:FM CONF
![diagram_fm](manual_images/diagram_fm.jpg)

The synth has 2 x 4 operator FM engine. OSC1 or OSC2 can be set to FM mode.
Each operator has sine wave.
OSC1 and OSC2 share the FM parameter.
On top of two FM engines, you can do FM modulation between oscillators.

1. FM ALGORITHM

	Selects FM algorithm. "ABCD" indicates each operator.
	Vertical relationship means upper operator modulates lower operator.
	For example,
```
	    A
	B C D
```
	This means that operator A modulates operator D. B, C and modulated D will be mixed in parallel.
```
	A
	B
	C
	D
```
	This means A modulates B, the result modulates C, the result modulates D.

2/4/6/8. FM (ABCD) AMP

	Oscillator (ABCD)’s amplitude.

3/5/7. FM (ABC) FREQ

	Oscillator (ABC)’s frequency (multiple of frequency of D)
	When FM FREQ SNAP (In ENV3/4 Other sub-menu) is off, it be adjust to the exact frequency of harmonics (2,3,4,5..). If you want clean FM sound, turn FM FREQ SNAP on.

### PRM:ENV3/4 / Other

1. 2ND FILTER

  Second filter can be used when you use 2 pole filter for VCF.

Mode | Description
------------ | -------------
NC200 | Notch filter at 200Hz. It will remove some muddy.
NC1K | Notch filter at 1kHz. It will remove some highs.
LS100 | Low-shelf at 100Hz. It will boot bass without cutting high.
LS150 | Low-shelf at 150Hz. It will boot bass without cutting high.
LS200 | Low-shelf at 200Hz. It will boot bass without cutting high.
LS300 | Low-shelf at 300Hz. It will boot bass without cutting high.
HP80 | Highpass at 80Hz. It will remove low-end bass to get more clear sound.
LP4K | Lowpass at 4kHz. It will remove high-end.
PK100 | Peak filter at 100Hz. Similar to band-pass filter, but Peak filter boots the peak frequency but it will not cut other frequency like band-pass filter.
PK150 | Peak filter at 150Hz.
PK200 | Peak filter at 200Hz.
PK300 | Peak filter at 300Hz.
PK400 | Peak filter at 400Hz.
PK800 | Peak filter at 800Hz.


2. FM FREQ SNAP SW

	Frequency snapping for FM. When it's ON, FM sound will be clear, no detune.
	When it's OFF, FM has more character, the signature sound of the QUN synth.

3. Clipping

	Clipping algorithm. "GRAIN", "MID" or "SOFT". The clipping algorithm will give a good distortion sound, you can even use the synth as multi-effector. See "External Audio processing" for further details.

4. FM ENV3 CONN

	Select operator(s) to connect ENV3
		FM engine's operators can use Envelope generator (ENV3/ENV4).
	Part of Operators can be connected to ENV3. The connection is configurable by this parameter.
	Technically ENV4 exists for OSC2’s FM engine, but the parameter is shared with ENV3.
	After the processing it will be modulated by ENV1 or ENV2.

5. ENV3/4 ATTACK

6. ENV3/4 DECAY

7. ENV3/4 SUSTAIN

8. ENV3/4 RELEASE

## PLAY MODE

![screen_play](./manual_images/screen_play.png)

Disk access indicator is active when system is accessing SD card. Some actions are restricted while writing.

Track / Scene tile shows selected track (A,B or C) and Scene number (1 to 5).

Looper status shows Looper position and status.

Clipping indictor is active when signal is clipped at the end of signal chain, after compressor.

### COMMON SEQUENCER / LOOPER OPERATIONS

Most of action works in any major mode, not limited to Play mode.

Button | function
-------|-------
SEQ PLAY | Start / Stop Sequencer
LOOPER PLAY | Start Looper
LOOPER STOP | Stop Looper
LOOPER REC + LOOPER PLAY | Start looper recording
SHIFT + SEQ PLAY + turn dial | Set BPM
LOOPER PLAY + [1-5] | Select Scene
REC + [1-3] | Select Track
PARAM + [1-3] | Mute track
PARAM + NO | Toggle Extra processing
MODE PLAY + [1-8] | Recall preset bucket
SEQ PLAY + [1-8] | Select Sequencer pattern
SEQ PLAY + NO / OK | Move to previous / next Sequencer page
SEQ PLAY + [1-8] + turn dial | Copy sequencer pattern to other bank. It's useful when you want to make a new bank by using existing data. If you want to cancel the operation, turn to the end, then "CANCEL" will be indicated as the destination. To initialize the bank data, turn the dial to "CLEAR". 
SEQ PLAY + [1-8] + NO / OK | Copy Sequencer page to previous / next Sequencer page
NO | Select previous pattern
OK | Select next pattern
SHIFT + LOOPER STOP | Delete all track recordings in the current scene, reset recording length 
REC + NO | CUT Looper track
REC + OK | PASTE Looper track
REC + PARAM | UNDO last recording for the track

### Sequencer overview

Tutorial video (https://www.youtube.com/watch?v=vZqdzkTQ1Mg)

The sequencer is an 8/16 step sequencer. One page has 8/16 steps and it can have up to 4 pages.

The sequencer UI is influenced by analog 8 step pattern based sequencer. You can on and off pattern and change parameters for the steps. 

Sequencer data will be saved when you save tone preset, and with the Session. Each preset can have 8 sequencer patterns.

### Looper overview

Tutorial video (https://www.youtube.com/watch?v=iD4WpX3tHUE)

The looper is designed to work with sequencer. The looper always tries to sync with sequencer play. Looper won't start playing when sequencer is not running. Use blank sequencer pattern when you don't want to make sound from sequencer.

To start looper recording, hit LOOPER REC + LOOPER PLAY. If the sequencer is not running, it will not start recording but it's stand by for recording. In this case, press SEQ PLAY to start recording. When the sequencer is playing, the recording will be started at the beginning of the next measure.

First recorded track will define the length of the loop.

Press LOOPER STOP when you finished the recording. You don't need to press the stop button precisely, you can press earlier, then recording will be finished at the end of the measure.

Looper keeps playing the recorded sound. All recorded data will be saved to SD card immediately.

Looper has 3 Tracks. REC + [1-3] button to select recording track. Each recording can go up to about 25 seconds.

One set of recordings is called Scene. Looper has 5 Scenes. LOOPER PLAY + [1-5] to select scene.

![looper_scene](./manual_images/looper_scene.png)

Reduce record volume (-3.0dB or more) in Mixer to avoid clipping. MODE PLAY + turn dial to change the value.

Cut / Paste can be used for temporary saved area or delete the track. REC + NO to Cut, REC + OK to Paste.

All recorded data, Preset bucket and Mixer data will be saved as a Session automatically. Recording data save immediately and other data will be saved when looper playing is stopped. Recording data is standard WAV file so you can import them to DAW.

### Looper live playing / Partial scene switch

Scene is powerful feature. You can play looper like Ableton Live's Session view. 
Play sequencer and looper, then LOOPER PLAY + [1-5] to select scene. Scene will be switched at the end of the measure. Synchronized switching works only when sequencer is playing.
You can switch Scene even if it's not the end of the recording. Changing point is the end of sequencer's measure.
Normally all tracks moves to new Scene, however, you can partially switch scene as well. Press LOOPER PLAY + [6-8] + [1-5]. [6-8] buttons tells which tracks you want to switch, and [1-5] is the scene number. Looper length can be different.
PARAM + [1-3] to mute tracks. 

Use Preset Bucket to keep preset settings. You can recall tone preset and patterns in a sec by using Preset Bucket.


### PLY:PLAY PIANO
The mode is simple piano playing mode. Default is chromatic scale, but the scale can be changed by the scale setting in SEQ Config mode. Turn dial to transpose.

### PLY:SEQ MODIFY
This controls modifier of the sequencer pattern.

Button | Function
------------ | -------------
1 | Pattern shuffle. 
2 | Transpose.
3 | Width Offset (note length). / Long press for playing Pattern shuffle
4 | Note Randomness
5 | Arpeggiator
6 | Rewind Period 
7 | Rewind Steps 
8 | Apply modifiers to the current sequence page 

The Modifier is powerful feature, it will give algorithmic effects to the pattern. Those effects will be applied to current pattern without breaking the pattern data.  Also you can apply modifiers to the pattern to make the effect as permanent.

- Transpose will add offset to the pattern. Scale quantize (SEQ Config button 3) will help to keep the result musical.
- Width Offset will change the note length.
- Randomness will add some randomness to playing notes.  Scale quantize (SEQ Config button 3) will help to keep the result musical.
- Arpeggiator will add note offset. Scale quantize (SEQ Config button 3) is important to generate usable Arpeggiator result.
- Pattern Shuffle will shuffle the playing order of the pattern. It is not random shuffle, so you can make creative and unexpected result without randomness.
- Rewind period and Rewind steps define the periodical rewind of the sequencer. However, the step goes back to 1 when playing count reaches the length of the pattern.

You can permanently apply the modifiers by pressing button 8. The result will be stored to selected sequence page. If you want to apply only partial steps of the page, you can press [1-8] buttons to unselect steps. Press OK to apply the modifiers while pressing [1-8] buttons. 

You will be asked resetting the modifiers or not resetting the modifiers. If you don't reset modifiers, then the modifiers will be reapplied to the result, so resetting modifiers is recommended to avoid confusions.

If the pattern has more than 8 steps, the modifier will be applied to only the current page. If you want to apply the modifiers to all pages, you don't want to reset modifiers.

After you applied the modifiers, the modifier values would be reset. Apply is powerful tool to create generative pattern.


### PLY:SEQ ON/OFF
The sequencer has 8 steps per page, but it has more modes than ON/OFF.
You can set different type of notes by turning dial while you press the button.

Status | Meaning
------------ | -------------
Left-filled circle | One note in the step.
Right-filled circle | One note in the step but it plays at the second half.
Fully-filled circle | Two notes in the step (1/16th).
Striped circle | 3 notes in the step (triplet).
Striped square | 4 notes in the step (1/32th)

### PLY:SEQ VELOCITY / WIDTH / PROBABILITY
Press one of the eight buttons and turn the dial, then it will modify velocity / width / probablity for each step.

If you press NO or OK while pressing [1-8] button, you can edit subdivision's parameter.

Index number | Meaning 
-------- | --------
0 | Main value, it will be used for the first-half note and other notes when other Index number is off
1 | 2nd half of the note (Used with 1/16th note)
2 | 3rd of the note (Used with triplet)
+0 | Main value for the second voice. Useful with Quad mode
+1 | 2nd half value for the second voice. Useful with Quad mode
+2 | 3rd value for the second voice. Useful with Quad mode

### PLY:SEQ TUNE
Press one of the eight buttons and turn the dial, then it will modify tune offset for each step.

If you press NO or OK while pressing [1-8] button, you can edit subdivision's parameter.

Index number | Meaning 
-------- | --------
0 | Main value, it will be used for the first-half note and other notes when other Index number is off
1 | 2nd half of the note (Used with 1/16th note)
2 | 3rd of the note (Used with triplet)
+0 | Main value for the second voice. Useful with Quad mode
+1 | 2nd half value for the second voice. Useful with Quad mode
+2 | 3rd value for the second voice. Useful with Quad mode
++0 | Main value for the 3rd voice. Useful with Quad mode
++1 | 2nd half value for the 3rd voice. Useful with Quad mode
++2 | 3rd value for the second voice. Useful with Quad mode
+++0 | Main value for the 4th voice. Useful with Quad mode
+++1 | 2nd half value for the 4th voice. Useful with Quad mode
+++2 | 3rd value for the 4th voice. Useful with Quad mode

#### Playing note capturing from external MIDI keyboard

Alternatevely, you can step record notes by external MIDI keyboard. Play note by MIDI keyboard while you are pressing one of the eight buttons, the note will be recorded as the tune for the step. Chord playing can be captured as well.
https://www.youtube.com/watch?v=aV2YL0idMHA

### PLY:SEQ CONFIG

Button | Function
------------ | -------------
1 | SWING. Long pressing the button for Sequencer MIDI channel out. 
2 | Key (for scale).
3 | Scale. Playing note will be quantized by this scale.
4 | Sequencer loop count. Default is 8.  
5 | BPM factor. Playing speed can be double or half.
6 | Velocity period (steps). You can play different velocity notes. Make sure you set Velocity Period Volume parameter and Velocity SW is ON
7 | Velocity Period Volume for off-beat note.
8 | Velocity Period Offset

Velocity period settings (Button 6 - 8) provide a convenient way to make rythmic velocity.

Sequencer MIDI channel out is useful setting with external synthesizer. When you set it, the sequencer starts to emit MIDI out signal to external synthesizers. Since it's the parameter of sequencer pattern, you can assign different MIDI channel for every single pattern.

## Ply: Granular

### Overview

The synth features a Granular synthesis recorder.
- Once you finish the editing, you can connect the Granular engine's output to AUX L channel. It means **Granular engine can be used as one of Oscillator shape**. You can assign Granular engine to Oscillator 1, and you still have Oscillator 2.
- You can record audio from LINE IN or MIC. Input sensitivity can be modified by "AUX In Gain" parameter.
- You can load audio from SD card.
- Pulse Width modulation will change File position (starting position) of the audio. That means the File position can be modulated by LFO and others.
- 4 Modes are available. **One shot, One shot with time stretch, Repeat, Repeat with time stretch**. When you are in One shot mode and play note slur, then the playing position won't be reset. 
- With One shot mode, you can route the signal to OSC1 AUX L and OSC2 AUX L. 
- Parameters can be controlled via MIDI CC. See the parameter start with GRN.
- With initialized state of oscillator, C4 is the original pitch of the audio.
- The number of voice is limited up to 2 voice with Granular mode.

This is a simple setup to use the granular engine:

1. Move to Granular sub mode, and record audio.
2. Adjust parameters in Granular mode
3. Change GRN mode from OFF to something else. It overrides AUX L channel to Granular engine's output.
4. Go Oscillator parameter page, and select OSC shape to "AUX L"
5. Play notes

### Operation

![diagram_grn](manual_images/diagram_grn.jpg)


Button | Function
------------ | -------------
1 | N/A 
2 | AUX Gain (This is the same parameter in Parameter mode, button 4 in Mix mode) 
3 | File position (Starting point).
4 | Length
5 | Speed. It won't work with non-time stretch modes.
6 | Number of Grain. It won't work with One-shot modes.
7 | Detune. (Octave highs and lows)
8 | GRN Mode. OFF, ONE(One shot), ONE_TS(One shot with time stretch), RPT(Repeat), RPT_TS(Repeat with time stretch). When the mode is not OFF, It will override AUX L signal to granular output when you use AUX L as Oscillator shape. With time stretch, playing speed will be preserved. Without it, pitch and speed are linked like an analog tape.
LOOPER REC + LOOPER PLAY | Start recording granular sample
LOOPER PLAY | Start playing 
LOOPER STOP | Stop playing
SHIFT + LOOPER REC | Save Recording data
SHIFT + LOOPER PLAY | Load Recording data

LOOPER buttons acts for granular in granular mode.

You can import WAV file if you put WAV file under /granular folder in SD card.
When granular mode is not OFF, the recording data will be save when you save preset, so normally you don't need to save recording data here. It's designed to export recording data.


### Granular synth tips

- Play note slur with One-shot mode. It works very well. You can keep the tempo with One shot with time stretch mode.
- PWM (Width) will change sample starting point, it will generate interesting result.
- Glide parameter is fun parameter with Granular.
- Speed can go negative.
- If you slice the audio to very short range with Repeat mode, the wave shape could be very simple and generic.
- With Repeat mode, set length to about 0.5 sec and changing Pulse Width makes unique sound.

### PLY:MIXER

Three track Mixer. At the last stage, signal can be **stereo** by panning tracks.

Button | Function
------------ | -------------
1 | Track A volume / Long press for Pan
2 | Track B volume / Long press for Pan
3 | Track C volume / Long press for Pan
4 | Record volume (After the clipper) / Long press for Pan
5 | Compressor threshold 
6 | Compressor makeup 
7 | Toggle extra processing (PARAM + NO is the shortcut)

This mixer has a compressor. Ratio, attack time and release time are fixed (1:3, attack 30ms, release 100ms).

To turn off compressor, set Compressor threshold to zero.

See clipping incidator if you want to avoid clipping. The synth does soft clipping, so the clipped sound is preferrable sometimes.

Mixer setting will be saved when Session is saved.

### Extra processing

You can toggle Extra processing mode by **PARAM + NO** button. 

When it's enabled, the Oscillators are turned off, but filter and effector becomes stereo, and connected to after Looper.
You can apply filter, filter volume, and effects against Looper recording. **See the signal diagram to understand how it works.**

LFO is still available for filter modulation.

The following parameters are still available with Extra processing:

- All parameters in VCF sub-mode
- VCF Mod Sel
- VCF Volume
- 2 / 4 pole
- 2nd Filter (When VCF is 2 pole)
- All parameters in LFO submode
-  Effector parameters (Type, Speed, Depth and Feedback)

## SYSTEM MODE

### Bank (1 to 8)

Load or save preset. Each bank can store up to 32 preset. Bank 7 and 8 is used for factory install preset, but you can edit it.

Button | Function
-------- | --------
SHIFT + LOOPER REC | Save
SHIFT + LOOPER PLAY | Load

Sequencer data will be stored with preset.
Granular record data will be saved when granular mode is not OFF.


### SYS:SYSTEM
System Setting is the setting that is not included in the patch setting. To change the parameter, press the one of 8 buttons and rotate the dial.


Button | Function
------------ | -------------
1 | Input source select / Long press for Send And Return
2 | Number of devices
3 | Device Index
4 | Receive MIDI Channel
5 | MIDI forwarding
6 | Line in through
7 | Line in HPF
8 | Sync mode


AUX: Input source select. Select Mic (the board has two onboard microphones) or Line in. The setting will be stored in the flash memory. When you use LINE IN, set this setting to "LINE IN(2CH)". You can record the source to granular engine.

Send And Return : OSC1 output before Envelope generator is coonnected to right channel. You need stereo channel separator to do this. Connection should the following:

     Qun's stereo output ->(stereo channel breakout cable, right channel)--(mono cable)--> effectors --(mono_cable)-> Qun's line in


Number of devices: Number of devices for poly mode. Set 1 if you don’t have multiple devices. It will be stored in the flash memory.

Device Index: Device Index. Set 1 if you don’t have multiple devices. It will be stored in the flash memory.

RECV MIDI Ch: Configure receiving MIDI channel. Default is ALL. If you use it with Polyphonic setup, set the same channel or ALL for all devices.

MIDI Forwarding: MIDI message forwarding for standalone polyphonic configuration. When the option is ON, the message forwarding is active with PolyMono or PolyQuad configuration. It's not for generic MIDI forwarding like MIDI THRU. Do not turn this option with DAW configuration. Most of DAW will echo received MIDI message, it will cause an infinite MIDI message loop. 

LINE in THRU: If it is off, it is automatically turn on or off LINE IN pass through by mono / poly setting. If it is on, the synth always passes the signal to looper. This setting will be stored in the flash memory. Gain is fixed to 1.

LINE in HPF: On is default. LINE in has two HPFs, one is external, one is internal HPF in the chip. This setting turns internal HPF. Turning this off will reduce HPF effect.

Sync Mode: `STOP, MIDI, 2PPQ, 4PPQ, 24PPQ, MOUT, MOUT2`. Select clock source for sequencer and LFO. See `Clock synchronization` for detail. 


### SYS:SYSTEM2

System2 is page 2 of system menu.
In System major mode, SHIFT + [OK] to go System2 menu.

Button | Function
------------ | -------------
1 | Quad mode On/Off

Quad mode enables quad voice (4 voices, 1 oscillator per voice) or dual-mono (2 voices, 2 oscillators per voice)
When the mode is off, voice will be Duo (2 voices, 1 oscillator per voice) or mono. Setting this mode will help to reduce system load.



## POLYPHONIC SETUP
The synth can be used as Mono or Quad(4) voice if you have one device.  Please see "MONO/QUAD/POLY (Voice mode)" section for detail.

The number of the voice can be increased if you have more than one device. Qun mk1 and mk2 has compatible sound engine. The voice number can be increased up to 16 (with Quad mode), by stacking up the synths.

_Tested well with two devices, using more than 2 devices is experimental at this stage._

### Audio connection

There are two ways for audio setup:

1. Connect Slave's audio out to Master's Line IN to combine outputs.
2. Connect all audio signals to your mixer.

### MIDI connection

Use TRS cable to connect Master's MIDI out to Slave's MIDI IN.

Turn on MIDI Forwarding in System menu. All received MIDI signal will be forwarded to Slave device. 

Please make sure you turn off MIDI forwarding when you connect MIDI OUT to DAW next time. Normally DAW echoes the received MIDI packet, so MIDI forwarding setting will cause MIDI message flood.

### Preset setup for Polyphonic

Minimum setup to achieve PolyMono (2 Oscillators per voice) will be the following with 2 devices setup:

1. In System menu, "Num of devices" should be 2 for all devices. Set Dev Index=1 for Master device, 2 for Slave device. This will be saved to flash memory.
2. Initialize a preset (SHIFT + PARAM) on Master device.
3. Make sure it plays initial SAW wave sound.
4. Go Key / Other sub-menu and set MonoQuadPolyMode to "PolyMono"
5. SHIFT + MODE PLAY button to dump all preset parameters as MIDI CC messages. After the dump, all preset state should be in sync between devices.
6. Play multiple notes. You should hear two voices.

Minimum setup to achieve PolyDuo (1 Oscillator per voice) will be the following with 2 devices setup:

1. In System menu, "Num of devices" should be 2 for all devices. Set Dev Index=1 for Master device, 2 for Slave device.
2. Initialize a preset (SHIFT + PARAM) on Master device.
3. Make sure it can play initial SAW wave sound.
4. Go Key / Other sub-menu and set MonoDuoPolyMode to "PolyQuad"
5. SHIFT + MODE PLAY button to dump all preset commands. After the dump, all preset state should be in sync between devices.
6. Play multiple notes. You should hear four voices.

### Polyphonic tips

Long press in Modo/Quad/Poly param (Long-press button 6 in Key/Other menu) to synchronize parameters between ocillators.

To synchronize all parameters between multiple Qun synthesizers, press SHIFT + MODE PLAY to dump all parameters. It will be sent to slave devices. If you still see issues like out of tune in slave device, try MIDI RECV toggle switch (SHIFT + SYSTEM). It will reset pitch bend or other controller values.


## TIPS/TROUBLESHOOTING

* Unknown MIDI messages sent with device reset?
  * When booting some noise is sent (it's ESP32's boot message) . Please avoid to receive MIDI signals when you reset the device. Use initializing preset (SHIFT +PARAM), instead of hardware reset.
* Trouble with Duo Mode: You need to set up properly to play duo mode properly.
  * Go Key / Other sub-menu and long press button 7. It will sync the parameters OSC1 and OSC2, it will resolve most of issues.
* No sound suddenly
  * Reset the preset. SHIFT + PARAM to initialize the preset.
  * Probably it’s because of last parameter you changed, or some unexpected MIDI cc signal. See the 2nd line of the display, it indicates the parameter received at last.
  * Level overflow may cause the silent, e.g. giving massive delay feedback.
  * Check "Device Index" and "Number of Devices" in system menu. If the Device Index is 2 or more, and you are using it as a primary device, then it may produce no sound. Set the index to 1.
  * Receiving MIDI channel is wrong. Check system setting.
  * Check MIDI Receiving status (Small Square dot in the screen. See PLAY MODE section for detail)
* A noise when you connect multiple devices (chained audio)

  * It is likely because of a ground loop. Use separated power supply. 
* Noise but nothing is connected to the line in.
  * Toggle MIC/LINE select (in System menu), set to Line in.
  * Toggle Line In THRU to off.
  * Initialize a preset.
  * Check Mono/Poly Mode setting. If it’s poly mode, LINE IN pass through turns ON.
* Use different power supply, you get less noise using separated charger.
* Don’t be afraid to get clipped! The synth has 3 great clipping algorithms. Clipping could be the gateway to a whole new sound.
* I want to use AUX as CV IN
  * CV signal from modular synthesizers may have **HIGH VOLTAGE**! Please attenuate the voltage to normal LINE level (1 to 1.5V).

  * AUX is connected to a lot of modules for CV control, so you can use AUX to control tune/width/LFO and others. However, the LINE in has capacitor in the path, it means the signal is AC. Using it as LFO should work, probably down to 2 to 5Hz. But DC signal, e.g. holding the same voltage 5 seconds, might not work.
* MIDI is flooding when I connect MIDI out to DAW.
  * MIDI forwarding is ON.
* Glithes with looper playing
	* One known issue is looper might get gliches when Granular's grain is high with scene loading. It's because of limitation of RAM bandwidth. 

## External Audio processing

You can use LINE IN signal for various purposes. LINE IN is stereo input.

* As CV input to control synth parameters
* As oscillator source. Select "AUXL" or "AUXR" as oscillator source. VCF / effector / Clipping will be applied. If you want to process LINE IN signal as an audio signal, then set Oscillator(1/2)'s signal as "AUXR" or "AUXL", and set the ENV SEL as "ON" (in OSC Switches). Set the gain by changing "VCF Volume" and "AUX In Gain" in Mix sub-menu. 
* ### Line In Through to Looper. Setting is in System -> Line In Through. It pass through the sound engine, then combined with the output of the sound engine. You can record the input to looper. Compressor will be applied.


## Clock synchronization

The synth can take external clock sources from other synthesizers. When the sync is enabled, sequencer BPM / start / stop is synchronized with external synthesizer or sequencer.
Setting is available in the System menu. Default is OFF. The setting will be saved to internal flash memory.

### MIDI clock
When you set sync mode to "MIDI", the synth will be clock slave mode. Set your DAW to send MIDI clock. We tested Ableton Live and Logic Pro X and KeyStep Pro. It has some latency so please adjust latency setting in your DAW to match the timing.

If you set sync mode to "MOUT" or "MOUT2", then the synth will be clock master. It sends MIDI clock as well as play/stop MIDI messages. Try "MOUT2" if you feel slight delay between devices. MOUT2 will send extra clock signal when start playing because some devices start sequencing from the second clock  (Roland MC-101is the example). If you clock another Qun, use MOUT.

### Sync IN
The synth can take 2PPQ, 4PPQ or 24 PPQ signals. Don't supply high voltage to the synth, it will break. The signal must be supplied to LEFT channel (tip of TRS connector). Using the tip as a sync signal is compatible with Teenage Engineering's Pocket Operator. Supply voltage needs to be more than 500mV. RIGHT channel (AUXR) still can be used as audio signal or CV in.

## SD card folder structure

WAV file can be used by other software. Format is mono, 48kHz, 16 bit.

### LOOPER00
Session data is stored here. It includes Looper recording data. 
Filename | Description
-------- | --------
[T000_1A.wav] | T means track recording, and next 3 digit is Session number, and 1 is Scene number, and A is track number. "0Z" is clipboard data. 
[M000_00.dat] | M means mixer data. The first 3 digit means Session number. The second 2 digit is always zero. 
[B000_00.dat] | B means Bucket data. This contains 8 preset and 64 sequencer pattern. The first 3 digit means Session number. The second 2 digit is always zero. 
[Z000_00.dat] | Z is for undo buffer.

When the directory has more than 500 files, then "LOOPER01" will be created.

### PRESET
Preset (Bank 1 to 8) is stored here.
Filename | Description
-------- | --------
[G_AAAAAA.WAV] | G means Granular record data. This is saved when Granular mode is not OFF.
[P_AAAAAA.DAT] | P means preset data.
[S_AAAAAA.DAT] | S means sequencer data. One file contains 8 pattern.

### GRANULAR
This is the place to export or import Granular record data. You can put your WAV file here to load the file to Granular engine. Format has to be 48000Hz, 16 bit, Mono.

Filename | Description
-------- | --------
[G_AAAAAA.WAV] | G means Granular record data. This is saved when You perform save command in Granular mode. If you save in Bank1 to Bank8 mode, Granular recording data is stored under Preset folder. 

### SSHOTS
Screnshots is stored here. To take screenshot, press LOOPER STOP + PARAM.

### IMPORT

Import is the folder to import loops to session.
Format has to be mono, 48kHz, 16 bit. See "Session" section for detail.


## Supported MIDI Control numbers

All tone-related parameters can be controlled by MIDI CC signal.

A set of MIDI CC signal can be used as preset save data. Press SHIFT + MODE PLAY button to dump MIDI CC messages.

If you want to control parameters by your MIDI keyboard, use the chart below to check the CC number.
Or, you can see the CC# in the screen at the top of the parameter name.
Assigned CC# can be override temporary.

When you change CC parameters through MIDI keyboard or any other devices, the changed parameter will be shown on the display in real-time, you will see what you are changing, the value and mode names just like when you change parameters directly on the QUN.

Suggested MIDI CC parameters to be assigned if your MIDI keyboard has some knobs:

- MIX: (92) 
- FM: (33)
- Cutoff: (22)
- Resonance: (91)
- LFO Tune: (24)
- VCF Volume: (90)




```
0                            "Save Preset", //0x0
1                            "Mod Wheel", //1
2                            "", //2
3                            "", //3
4                            "", //4
5                            "", //5
6                            "", //6
7                            "Volume", //7
8                            "", //8
9                            "", //9
10                            "", //a
11                            "VCF Volume", //b
12                            "", //c
13                            "", //d
14                            "", //e
15                            "", //f
                            //-----------------------0x10
16                            "", //0x0
17                            "", //1
18                            "", //2
19                            "", //3
20                            "", //4
21                            "OSC1 Tune(MSB)", //5
22                            "VCF Cutoff(MSB)", //6
23                            "OSC2 Tune(MSB)", //7
24                            "LFO Tune(MSB)", //8
25                            "ENV3/4 Attack", //9
26                            "ENV3/4 Decay", //a
27                            "ENV3/4 Sustain", //b
28                            "ENV3/4 Release", //c
29                            "GRN File Pos", //d
30                            "GRN Length", //e
31                            "GRN Speed", //f
                            //-----------------------0x20
32                            "GRN Grain", //0x0
33                            "FM", //1
34                            "Efct Feedback", //2
35                            "LFO Pulse Width", //3
36                            "OSC1 Pulse Width", //4
37                            "OSC2 Pulse Width", //5
38                            "LFO Pulse Width", //6
39                            "Efct Speed", //7
40                            "VCF Type", //8
41                            "Efct Depth", //9
42                            "OSC1 Bypass", //a
43                            "GRN Detune", //b
44                            "Efct Type", //c
45                            "VCF OSC1 bypass SW", //d
46                            "GRN Detune", //e
47                            "GRN Mode", //f
                            //-----------------------0x30
48                            "LFO Mod Tune", //0x0
49                            "LFO Mod Width", //1
50                            "FM Algorithm", //2
51                            "FM ENV3 Conn", //3
52                            "", //4
53                            "OSC1 Tune(LSB)", //5
54                            "Cutoff(LSB)", //6
55                            "OSC2 Tune(LSB)", //7
56                            "LFO Tune(LSB)", //8
57                            "FM A Amp", // 9
58                            "FM A Freq", //a
59                            "FM B Amp", //b
60                            "FM B Freq", //c
61                            "FM C Amp", //d
62                            "FM C Freq", //e
63                            "FM D Amp", //f
                            //-----------------------0x40
64                            "", //0x0
65                            "OSC2 Mod Sel", //1
66                            "LFO Mod Sel", //2
67                            "ENV1 Inv SW", //3
68                            "OSC1 Env Sel", //4
69                            "OSC2 Env Sel", //5
70                            "ENV2 Inv SW", //6
71                            "LFO Gatesync SW", //7
72                            "FM FREQ SNAP SW", //8
73                            "OSC1 Wide Tune SW", //9
74                            "OSC2 Wide Tune SW", //a
75                            "OSC2 Octave", //b
76                            "OSC1 Octave", //c
77                            "OSC1 Keysync SW", //d
78                            "Velocity SW", //e
79                            "OSC1 LFO Tune", //f
                            //-----------------------0x50
80                            "OSC1 LFO Width", //0x0
81                            "OSC2 LFO Tune", //1
82                            "OSC2 LFO Width", //2
83                            "Mono/Duo/Polly", //3
84                            "VCF LFO Volume", //4
85                            "VCF Mod Cutoff", //5
86                            "LFO Keysplit", //6
87                            "VCF LFO cutoff", //7
88                            "OSC1 Mod Sel", //8
89                            "VCF Mod Sel", //9
90                            "VCF Volume", //a
91                            "VCF Resonance", //b
92                            "OSC Mix", //c
93                            "OSC1 Shape", //d
94                            "OSC2 Shape", //e
95                            "LFO Shape", //f
                            //-----------------------0x60
96                            "ENV1 Attack", //0x0
97                            "AUX In Gain", //1
98                            "", //2 (Won't be dumped)
99                            "", //3 (Won't be dumped)
100                            "Mod Wheel Mode", //4
101                            "", //5 (Won't be dumped)
102                            "ENV1 Decay", //6
103                            "ENV1 Sustain", //7
104                            "ENV1 Release", //8
105                            "ENV2 Attack", //9
106                            "ENV2 Decay", //a
107                            "ENV2 Sustain", //b
108                            "ENV2 Release", //c
109                            "OSC1 Mod Tune", //d
110                            "OSC1 Mod Width", //e
111                            "VCF Pole / NoLinear", //f
                            //-----------------------0x70
112                            "OSC2 Mod Tune", //0x0
113                            "OSC2 Mod Width", //1
114                            "Glide", //2
115                            "Bend Range", //3
116                            "Mod Mode", //4
117                            "VCF Keysync", //5
118                            "Voice Number", //6
119                            "LFO Sync SW", //7
120                            "All Notes Off", //8
121                            "", //9
122                            "", //a
123                            "All Notes Off", //b
124                            "", //c
125                            "", //d
126                            "", //e
127                            "" //f
```
## Quick Setup with Third-party Software & Hardware
The QUN synth can be setup quickly for use with third-party software and hardware by downloading the appropriate configuration file from [Configurations](./configurations). The following configurations files are currently available:

* Native Instruments Maschine
* Native Instruments Komplete Kontrol
