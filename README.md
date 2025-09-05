# ICARIZ-FINAL-SUBMISSION
Assumptions:
1)The solar panels and the MPPT are treated as a single power source that provides about 6 W during the sun period.
2)The battery is an ideal voltage source with a small series resistance to simulate voltage droop under load.
    Voltage Source: Set to 7.4 V.
    Series Resistor: A small value like 50 mΩ
3)This represents energy lost in wiring and voltage converters. A simple series resistor is the easiest way to model this.
Component Choice: A Resistor.Value:100 mΩ  
4)Model the Loads
   A)Load 1: OBC/Housekeeping (Always On)
         Assumed Power: 1 W (constant background load).
         Resistance: R=V^2*I=55 Ω
         ON time=Always
    B)Load 2: TT&C (Short Bursts)
          Assumed Power: 4 W (high power radio transmission).
          Resistance: R=14 Ω 
          ON time= from from t=100s to t=400s
    C)Load 3: Payload (Sun-Only)
          Assumed Power: 2 W.
          Resistance: R=27 Ω  from t=0 to t=3600        
    
