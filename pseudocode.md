# Washing your Hands
## INIT Objects/Var/assumptions

1. **faucet**
    * automaticSensorFaucet
    * manualFaucet
2. **soapDispenser**
    * automaticDispenser
    * manualPump
    * manualPush
3. **objectToDry**
    * handTowel
    * Hand dryer
        - automaticDryer
        - manualButton
4. **scrubHands**

5. **warmWaterKnob**
---
## Functions

### **Function prepareToWash**
>* **IF** sink = automaticSensorFaucet
>   - **THEN** Place hands under faucet.
>       - **ELSE** Turn warmWaterKnob to *on* position.<br>
   >   **END**
>* Wet hands with water from faucet.

### **Function applySoap** 

>* **IF** soapDispenser = manualPush
>* **THEN** Use palm of hand to push button to dispense soap into your hand.
>   - **ELSE IF** soapDispenser = manualPump.
>   - **THEN** Place one hand under dispenser and use other hand to pump the lever dispensing soap.
>       * **ELSE** Place hand under sensor to dispense soap.<br>
    **END**
   
### **Function washHands**
>* Rub hands together to lather soap covering entirety of hands.
>* Scrub hands vigorously.
>*  **LET** scrubHands = 0seconds.
>       - **DO** (scrubHands++)
>           -  **WHILE** (scrubHands < 20seconds) <br>
>   **END**

### **function rinseHands**
>* Place hands under water to rinse off soap.
>   - **IF** Soap is gone.
>   * **THEN** turn warmWaterKnob to *off* position.
>       - **ELSE** continue rinsing until soap is gone then turn warmWaterKnob to *off* position.

### **function dryHands**
>* **IF** objectToDry = automaticDryer
>* **THEN** Place hands under sensor to start dryer and hold until dry.
>      - **ELSE IF** objecToDry =  manualButton
>      - **THEN** press button to start and place hands under dryer until dry.
>           * **ELSE** Remove handTowel from rack. Use handTowel to dry hands. Place back on towel rack.<br>
**END**

----
## **PSEUDOCODE**
//Begin Program

INIT()

functionPrepareToWash()

function applySoap()

function washHands()

function rinseHands()

function dryHands()

//End Program





    
                


       
