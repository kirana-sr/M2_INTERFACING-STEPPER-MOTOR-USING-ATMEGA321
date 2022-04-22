# Report#


1.INTRODUCTION **
Stepper Motors are DC brushless vehicles that could rotate from zero to 
360 in steps. Stepper motor makes use of digital alerts to rotate the motor 
in steps and every sign rotates the shaft in constant increment (one step). 
The rotation angel is managed with the aid of using making use of positive
series of signals. Unlike Servo Motor, stepper cars may be pushed with the 
aid of using the usage of GPIO pins of microcontroller in place of PWM pins 
and might rotate in (+360) and (-360). 
The order of indicators makes a decision the clockwise and counter 
clockwise route of stepper motor. To manipulate the rate of the motor, we 
simply want to extrade the price of manipulate indicators applied. The 
stepper automobiles rotates in steps. 
There are numerous modes of steps to function Stepper Motor along with
complete step, 1/2 of step and micro step. We will interface 28BYJ-forty 
eight Stepper Motor with Atmega328 AVR Microcontroller the use of Atmel 
Studio 7.0. 
The stepper motor is rated to paintings in 5V. We can be interfacing the 
stepper motor with each the motor drivers i.e. ULN2008. Both can be
pushed with the aid of using 5V supply. In order to simplify the interfacing 
we're the use of prebuild module of each motor drivers. We also can use 
ULN2003 and L293D standalone IC’s. The wide variety of wires and 
jumpers may be more, so simply be cautious at the same time as
connecting all of the connections.
A stepper motor is a form of DC motor that rotates in steps. When electric
sign is implemented to it, the motor rotates in steps and the velocity of 
rotation relies upon at the charge at which the electric indicators are 
implemented and the route of rotation is depending on the sample of pulses 
this is followed.
A stepper motor is made from a rotor, that's usually a everlasting magnet 
and it is, because the call indicates the rotating element of the motor. A 
stator is some other component that's with inside the shape of winding. In 
the diagram below, the centre is the rotor that's surrounded with the aid of 
using the stator winding. This is referred to as 4 section winding.

 METHODOLOGY 
2.1 HARDWARE COMPONENT 
 1. STEPPER MOTOR 
 2. ULN2008 
 3. ATMEGA328 
 4. RESISTER 
 5. SWITCH 
 6. GROUND 
7. CONNECTING WIRES
 
2.1.1. STEPPER MOTOR 

![image](https://user-images.githubusercontent.com/101106080/164648344-ea2916ad-6e55-491e-a1b3-bf6967d8ec9d.png)

The centre faucet at the stator winding permits the cutting-edge with inside the coil 
to extrade path whilst the winding are grounded. The magnetic belongings of the 
stator adjustments and it's going to selectively entice and repel the rotor, thereby 
ensuing in a stepping movement for the motor

Stepping Sequence 
In order to get accurate movement of the motor, a stepping collection needs to be
accompanied. This stepping collection offers voltage that need to be carried out to 
the stator phase
Normally a four step collection is accompanied. When the collection is 
accompanied from step 1 to four, we get a clock clever rotation and whilst it's far
accompanied from step four to 1, we get a counter clockwise rotation 
The pin connections for OUTPUT are as follows:


![image](https://user-images.githubusercontent.com/101106080/164648709-ef280418-ec61-4888-8e7b-d61f72fb8bac.png)

2.1.2. ULN2008 
Connect all of the additives as proven with inside the diagram beneath whilst the 
use of ULN2008. Similarly we can be interfacing it the use of L293D in 
subsequent step. We are the use of PORTA of Atmega328 to interface stepper 
motor for each the motor drivers. 
There isn't any want to attach the 5V pin of stepper motor. Only the coil pins are 
required to transport the stepper motor. The pin order could be very crucial to force
stepper motor because the energizing of the coils must be for you to gain steps. 
Four inputs of ULN2008 and 4 outputs of ULN2008 are used on this project t. 
The inputs may be related to PORTA pins and outputs may be related to Stepper 
Motor Signal pins. I Also, join one push button in Reset pin for resetting 
Atmega16 each time required. Connect Atmega16 with right crystal oscillator 
circuit. All the machine may be powered through 5V supply

![image](https://user-images.githubusercontent.com/101106080/164648904-bc84794c-77c9-4c29-b11c-16d5e392e91c.png)

The pin connections for INPUT are as follows:


![image](https://user-images.githubusercontent.com/101106080/164649108-1668cab8-e306-4b95-afdf-a5476e87501a.png)

2.1.3. ATMEGA328 
The high-overall performance Microchip Pico Power 8-bit AVR RISC-primarily 
based totally microcontroller combines 32KB ISP flash reminiscence with readwhile-write capabilities, 1024B EEPROM, 2KB SRAM, 23 fashionable-motive I/O 
lines, 32 fashionable motive running registers, 
Three bendy timer/counters with examine modes, inner and outside interrupts, 
serial programmable USART, a byte-orientated 2-cord serial interface, SPI serial 
port, a 6-channel 10-bit A/D converter (8-channels in TQFP and QFN/MLF 
packages), 
Programmable watchdog timer with inner oscillator, and 5 software program
selectable energy saving modes. The tool operates among 1.8-five.five volts. 
By executing effective commands in a unmarried clock cycle, the tool achieves 
throughputs drawing close 1 MIPS according to MHz, balancing electricity intake
and processing speed


![image](https://user-images.githubusercontent.com/101106080/164649528-c309386b-cee9-4f71-a6d5-b2edede7541d.png)

ATmega328 has 1KB Electrically Erasable Programmable Read-Only Memory 
(EEPROM). This belongings indicates if the electrical deliver furnished to the 
micro-controller is removed, even then it is able to keep the statistics and may offer
effects after supplying it with the electrical deliver. Moreover, ATmega-328 has 
2KB Static Random Access Memory (SRAM). 
The high-overall performance Microchip Pico Power 8-bit AVR RISC-primarily 
based totally microcontroller combines 32KB ISP flash reminiscence with readwhile-write capabilities, 1024B EEPROM, 2KB SRAM, 23 standard-reason I/O 
lines, 32 standard reason running registers 
Three bendy timer/counters with examine modes, inner and outside interrupts, 
serial programmable USART, a byte-orientated 2-cord serial interface, SPI serial 
port, a 6-channel 10-bit A/D converter (8-channels in TQFP and QFN/MLF 
packages),
Programmable watchdog timer with inner oscillator, and 5 software program
selectable strength saving modes. The tool operates among 1.8-five.five volts.
By executing effective commands in a unmarried clock cycle, the tool achieves 
throughputs drawing near 1 MIPS in step with MHz, balancing strength intake and 
processing speed. 
To maximize overall performance and parallelism, the AVR makes use of a 
Harvard architecture – with separate recollections and buses for software and data. 
Instructions withinside the software reminiscence are completed with a unmarried
stage pipelining. While one training is being completed,
The subsequent coaching is pre-fetched from this system reminiscence. This idea
allows commands to be performed in each clock cycle. The software reminiscence
is in-gadget reprogrammable flash reminiscence

4. RESISTER 
Resistor is defined as the main purpose of resistor is to reduce the current flow 
and to lower the voltage in any particular portion of the circuit. It is made of copper 
wires. Which i is coiled around a ceramic rod and the outer part of the resistor is 
coated with an insulating paint.

5. SWITCH 
The Reload feature of the Cisco Small Business Switches is beneficial whilst
positive modifications with inside the settings require a reboot to absolutely
follow the configuration settings, or if the tool isn't always functioning as 
expected. The configuration settings of the community tool get meditated
after the tool restarts.

The Reset function is used to take away the strolling or modern-day
configuration settings at the community tool and repair it to the authentic
default settings. Manual reset is suggested while the complete tool desires to 
be reconfigured, or if you overlook the password and now no longer capable 
of get better through any method along with gaining access to the console the 
use of Telnet, Secure Shell (SSH), or Command Line Interface .

6. GROUND 
The grounding gadget is a "backup" pathway that offers an change direction for 
electric modern to observe lower back to "ground" with inside the case of a trouble
with inside the wiring gadget.

7. CONNECTING WIRES 
Connecting wires lets in an electrical cutting-edge to tour from one factor on a 
circuit to another, due to the fact strength desires a medium via which to move. In 
the case of computers, wires are embedded into circuit boards,

CIRCUIT DIAGRAM 


![Screenshot 2022-04-22 130205](https://user-images.githubusercontent.com/101106080/164650026-7d7773cd-df6f-407c-89c1-3bac61d07089.png)
WORKING 
Stepper motor is a brushless DC motor that divides the total rotation attitude of 
360° into some of identical steps.
 • The motor is turned around through making use of a sure series of manipulate
alerts. The pace of rotation may be modified through converting the fee at which 
the manipulate alerts are applied. 
• Various stepper cars with one-of-a-kind step angles and torque rankings are to be 
had with inside the market. 
 • A microcontroller may be used to use one-of-a-kind manipulate alerts to the 
motor to make it rotate consistent with the want of the application. 
• Here we're going to interface 6 wires Unipolar Stepper Motor with ATmega32 
controller 
. • Only 4 wires are required to manipulate the stepper motor. Two not unusual 
place wires of stepper motor related to 5V supply 
• ULN2003 driving force is used to the using stepper motor. 
 • Note that to recognize winding coil and their middle faucet leads degree
resistance in among leads. From middle leads, we are able to get 1/2 of the 
resistance price of that winding .

program 
#define F_CPU 8000000UL /* Define CPU Frequency 8MHz */
#include <avr/io.h> /* Include AVR std. library file */
#include <util/delay.h> /* Include delay header file */
{ 
int period; 
 DDRD = 0x0F; /* Make PORTD lower pins as output */
 Period = 100; /* Set period in between two steps */
While (1) 
 { 
 /* Rotate Stepper Motor clockwise with Half step sequence */
 For (int i=0; i<12;i++) 
 { 
 PORTD = 0x09; 
 _delay_ms (period); 
 PORTD = 0x08; 
 _delay_ms (period);
PORTD = 0x0C; 
 _delay_ms (period); 
 PORTD = 0x04; 
 _delay_ms (period); 
 PORTD = 0x06; 
 _delay_ms (period); 
 PORTD = 0x02; 
 _delay_ms (period); 
 PORTD = 0x03; 
 _delay_ms (period); 
 PORTD = 0x01; 
 _delay_ms (period); 
 } 
 PORTD = 0x09; /* Last step to initial position */ 
 _delay_ms (period); 
 _delay_ms (1000); 
 /* Anticlockwise with Full step sequence */
 for(int i=0;i<12;i++) 
 { 
 PORTD = 0x09; 
 _delay_ms (period); 
 PORTD = 0x03; 
 _delay_ms (period); 
 PORTD = 0x06; 
 _delay_ms (period); 
 PORTD = 0x0C; 
 _delay_ms (period); 
 } 
 PORTD = 0x09; 
 _delay_ms(period); 
 _delay_ms(1000); 
 } 
}

ALGORITHM 


![image](https://user-images.githubusercontent.com/101106080/164650425-46ef4c1a-e83a-4f4c-b9dc-ffb1e1311b75.png)
CONCLUSION 
The stepper motor may be turned around immediately with the aid of using
connecting the motor with the energy supply. But with the aid of using growing an 
Atmega software wherein the stepper motor may be turned around with the aid of 
using the usage of the ATMEGA microcontroller. The velocity and the rotary 
guidelines may be managed with the aid of using modifying iprogram. These c 
programming stepper automobiles may be specifically relevant withinside the
industries for the automation method. Generally stepper automobiles may be used 
for numerous applications. But with the aid of using programming and rotating the 
stepper motor, it is able to be relevant for automation method withinside the
industries.
REFERENCE 
[1] E. M. C. Wong, “A phone-primarily based totally faraway controller for domestic and 
workplace automation,” IEEE Transactions on Consumer Electronics, vol. 40, no. 1, pp. 28-34, 
Feb. 1994. 
 [2] N. Sriskanthan and Tan Karand, “Bluetooth Based Home Automation System”, Journal of 
Microprocessors and Microsystems, Vol. 26, pp.281-289, Elsevier Science B.V., 2002. 
 [3] Mandeep Singh, Rekha & Balwinder Singh, “Microcontroller Based Clockwise/Anticlockwise 
Stepper Motor Controller Using PC Keyboard Via Com Port”, International Journal of Computer 
Science & Communication Vol. 1, No. 1, JanuaryJune 2010, pp. 189-19



