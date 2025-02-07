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

Performing DC analysis, without any without selecting any components, we calculated the values of UnCox and UpCox using the  https://latex.codecogs.com/svg.image?\beta&space;_{eff} values we got from the DC operating points.
