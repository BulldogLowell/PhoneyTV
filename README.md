* PhoneyTV V3.0
 * by Jim  >> BulldogLowell@gmail.com
 * Inspired by Josh >> Deltanu1142@gmail.com
 *
 * This Sketch illuminates 6 sets of LED's in a random fashion as to mimic the 
 * ambient light eminating from a television.  It is intended to make an empty
 * home (or an empty section of a home) appear to be occupied by someone watching
 * TV.  As an alternative to a real television left on, this uses less than 1%
 * of the electrical energy.
 *
 * With the use of the MySensors plugin and gateway, PhoneyTV is intended to 
 * be used with Vera or Raspberry PI.
 *
 * Sketch does not use any delays to create the random blinking as a way to 
 * assure that communication back to the gateway is as unaffected as possible.
 *
 * You can adjust the length of the blink interval and its "twitchyness" by
 * modifying the random number generators, if you prefer more/less 'motion' in
 * in your unit.  The lines are highlighted in the code.
 *
 * Sketch takes advantage of available PWM on pins 3, 5 & 6 using the wht/blu LEDs 
 * to allow fluctuations in the intensity of the light, enhancing the PhoneyTV's
 * natural ambient light effect.
 *
 * This uses the MySensors.org sketch and will attach itself to your gateway as
 * a light, which was another requirement.  Because of that requirement, it 
 * utilizes one digital output pin in the logic (but not physically) and a relay
 * is not actually required to use this sketch.  Also, the radio pinout remains
 * in tact as to preserve the ease of use for MySensor.org users
 *
 * Created 12-APR-2014
 * Free for distrubution
 * Credit should be given to MySensors.org for their base code for relay control
 * and for the radio configuration.  Thanks Guys.
 *
 * 29-May-2014
 * Version 2:  Simplified the code, removing all redundant relay setup from original 
 * code.  Added an on/off momentary pushputton option to be set up on pin 2.  Inproved  
 * the dark dips for longer duration (can be configured) at intervals.
 *
 * 4-Oct-2014
 * Version 3:
 * Updated for MySensors V1.4
 *
 * 5-Nov-2015
 * Version 3.1: Turned off Relay functionality of node to eliminate network complexity
 * Updated for MySensors V1.4.1
 *
 */
