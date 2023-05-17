

# Mixing and Heating of Liquid Components

## Description

This project involves the control and management of a technological system that includes two identical tanks for mixing liquid components and temperature control. Additionally, there is a receiving tank (not shown in the task description) with a smaller volume compared to the combined volume of the two mixing tanks.

## Functionality

- Upon pressing the "Start" button, the valve for the first product's intake opens.
- After reaching the intermediate level, the valve for the first product closes and the valve for the second product's intake opens.
- Upon triggering the high-level alarm, the valve for the second product's intake closes, and the steam valve opens at 100%.
- Once the temperature reaches 95 degrees Celsius (within a sensor range of 0-150 degrees), the steam valve remains open at 20% for an additional 10 seconds.
- After the holding period, the liquid is drained from the apparatus.
- The cycle repeats if the stop button is not pressed. Pressing the stop button closes the drain valve.
