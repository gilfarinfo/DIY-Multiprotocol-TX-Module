# 

Modifications to maple mini

Multiprotocol.ino near line 35 

#if defined (ARDUINO_AVR_XMEGA32D4) || defined (ARDUINO_MULTI_ORANGERX)
	#include "MultiOrange.h"
#endif

//To run with maple mini board#if defined BOARD_maple_mini
#if defined BOARD_maple_mini
  #define STM32_BOARD
  #define ARDUINO_GENERIC_STM32F103C
#endif

#include "Multiprotocol.h"

Pins.h


Pins.h

near line 217

  #if defined BOARD_maple_mini
  #define BIND_pin    PA0 
  //la led pourra devenir 
  #define	LED_pin			PB1
 #else
  #define BIND_pin    PA0
  #define LED_pin     PA1
 #endif
 
 near line 240
 
   #if defined BOARD_maple_mini
    #define A7105_CSN_pin PA14               //A7105
  #else
	  #define	A7105_CSN_pin	PB9								//A7105
  #endif
  
near line 253

 #if defined BOARD_maple_mini
  #define RX_INV_pin    PB0
 #else
	#define	RX_INV_pin		PB1
 #endif
