# modwtpy
## MODWT in python

Detail from the matlab Documentation:
- http://www.mathworks.com/help/wavelet/ref/modwt.html,
- http://www.mathworks.com/help/wavelet/ref/modwtmra.html

The wavelet is imported from pywt:
http://www.pybytes.com/pywavelets/ref/wavelets.html

## Example
```python
from modwt import modwt, modwtmra
import pandas as pd


gdpdata = pd.DataFrame.from_csv('GDPcomponents.csv')
wt = modwt(gdpdata['govtexp'], 'db2', 5)
wtmra = modwtmra(wt, 'db2')
```
