# puredata-synth

Some synthesizers for PureData (mostly with arduino physical controls)

# Hardware description

- Arduino with a bunch of potentiometers attached to all the analog inputs
- running a very simple "Firmata" component
- connected with USB to the laptop I have PureData running on

# Reading
- Overview: description of doing this same thing:
    - https://spencerdixon.wordpress.com/2010/12/15/how-to-build-a-midi-controller-with-the-arduino-firmata-and-pure-data/
    - http://playground.arduino.cc/Interfacing/PD
- PureData software synthesizer, aka "Pd"
    - https://puredata.info/
- Arduino: connect a potentiometer
    - http://www.arduino.cc/en/Tutorial/Potentiometer

# Install

To get these running you will need:

- Pd-extended
    - http://puredata.info
    - some of Pduino needs extended libraries here
    - You may see an error message about X11: here's how to fix it on OSX
        - https://puredata.info/docs/faq/how-do-i-fix-this-error-library-not-loaded-usr-x11r6-lib-libx11-6-dylib 
- Pduino 
    - https://puredata.info/downloads/pduino/releases/0.5.beta8
    - this is a PD control that models an arduino connected with Firmata
    - tested with 0.5
    - include it in your library path for Pd
- Firmata
    - this is Arduino software which will get the knob values to the USB
    - tested with 2.2
    - Pd need not know about this part!


