# Analog-Circuit-Design-for-a-Common-Source-Amplifier-with-Current-Load
Designed a simple amplifier with a supply voltage of 3V and output swing of 2.2V at transistor level using UMC 55nm technology library in Cadence Virtuoso

![Screenshot 2025-02-07 190905](https://github.com/user-attachments/assets/9f580c37-4979-4366-887e-2d55a368e52c)

Av(theoretical) =100
Av(achieved)=63.9
Id = 1mA
Vdd = 3V
Output Swing = 2.2V

Rule of thumb , Vout = Vdd/ 2 = 1.5V 

3V - 2.2 V = 0.8 V
Therefore we assume the drop across pmos = 0.4V and nmos=0.4V (Vdsat)

To calculate bias voltage for pmos (Vb),
Vdsat =0.4V = Vsg - Vth = 3V - Vb -|-0.5|
Implies that , Vb = 2.1 V

To calculate gate voltage for nmos(Vg),
Vdsat = 0.4V = Vgs - Vth = Vg-0-0.5
Implies that , Vg =0.9 V

![Screenshot 2025-02-07 191235](https://github.com/user-attachments/assets/91fba7b9-c4a6-45c7-9262-09a9d24e0a37)

Using theoretical calculations we got, 
(w/l) pmos = 210.85
(w/l) nmos = 185.45

To get the w/l ratios for the pmos and nmos , we performed dc analysis of Id versus w, when we fixed the length = 500nm for nmos and 400 nm for pmos respectively.

Pmos width = 111.362um
Nmos width = 76.49um 

For ac analysis, we used
Frequency = 1kHz
AC Magnitude = 1

Results of AC analysis, Av =63.9

![Screenshot 2025-02-07 191320](https://github.com/user-attachments/assets/cf21c923-d50e-4f70-835f-cda714f733e7)
