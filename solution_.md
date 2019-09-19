MCC Van Dyke et al., 2019
* The Rise of Coccidioides: Forces Against the Dust Devil Unleashed
* Fantastic yeasts and where to find them: the hidden diversity of dimorphic fungal pathogens

JT Harvey, Applied Ergonomics, 2002
* An analysis of the forces required to drag sheep over various surfaces

DW Ziegler et al., 2005
* The neurocognitive effects of alcohol on adolescents and college students

``` python
import pandas as pd
import matplotlib.pyplot as plt

data = pd.read_csv("istherecorrelation.csv", delimiter=';')

plt.plot(data['Year'],data['NL Beer consumption [x1000 hectoliter]'], '--bo')
plt.xlabel('Year')
plt.ylabel('NL Beer Consumption [x1000 HL]')

plt.twinx()
plt.plot(data['Year'],data['WO [x1000]'], '--ro')
plt.ylabel('Number of WO students [x1000]')

plt.savefig('isthecorrelation.png',dpi=400,bbox_inches='tight')

plt.show()
```