# Acid Rain Prelab
Benjamin Lee and Wesley Sluga


```python
  from aguaclara.core.units import unit_registry as u
  import numpy as np
  import matplotlib.pyplot as plt
  import pandas as pd
  import math
  from scipy import stats

ANCin = 10**(-3)
ANCout = 50*10**(-6)
ANCo = (ANCout + ANCin *(1 - math.exp(-3))) * math.exp(3)
MolarMassNaHCO3 = 84
LakeVol = 4
MassNaHCO3 = ANCo*MolarMassNaHCO3*LakeVol
print(MassNaHCO3)
```
6.75 grams of NaHCO3 is required to keep the ANC levels in a lake above 50 μeq/L for 3 hydraulic residence times given an influent pH of 3.0 and a lake volume of 4 L, if the current lake ANC is 0 μeq/L.
