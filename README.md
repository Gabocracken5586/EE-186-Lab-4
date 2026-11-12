# EE-186-Lab-4
ADC:
Question 1:
In our Nucleo Board, the different bit resolutions that we can set for the ADC
are 12, 10, 8 or 6-bit.
Further, on page 214 of the datasheet, we found the maximum sapling rate for each one 
of these resolutions
    In the FAST channels:
    Resolution = 12 bits has a maximum sampling rate of 5.33Msps
    Resolution = 10 bits has a maximum sampling rate of 6.15Msps
    Resolution = 8 bits has a maximum sampling rate of 7.27Msps
    Resolution = 6 bits has a maximum sampling rate of 8.88Msps

    In the SLOW channels
    Resolution = 12 bits has a maximum sampling rate of 4.21Msps
    Resolution = 10 bits has a maximum sampling rate of 4.71Msps
    Resolution = 8 bits has a maximum sampling rate of 5.33Msps
    Resolution = 6 bits has a maximum sampling rate of 6.15Msps

Question 2:
The voltage dividers are used for the binary approximatoin of analog to digtial
conversion. It helps us to divide our reference voltage in multiples of 2 
as we approach the desired value. Without a voltage divider, the votlage at any point measured would consistently stay at 3.3v regardless fo the resistance being emited by the photoresistor. 

DAC:
Question 3:
Based on the equation that describes Vout = B/(2^n) * Vref. wE can plug in 9 for B and 12 for n as the best resoution for our MCU is 12 bits. After solving, it can be determined that Vout = 0.0022 * Vref.

Question 4: 
Because analog signals are continious, we can not store infinite data about a signla. Thus, we sample at a specific rate depending on the desired quality of the output. The highest the sampling rate the better is the quality of the signal as we have more data point to rebuild from. However, it is also a balance between performance of the machiens collecting the data points. 
The sound produced by the different waves varies as sin waves contain only one single fundamental frequency, which square waves contain only odd components, and the Sawtooth wave contains both odd-and-even. 
Lasltly, we need a capacitor in the signal path to serve as a low pass filter for filtering out high frequencies.
