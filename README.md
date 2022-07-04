# Linear Regression [![gcash donation][1]][2] [![paypal donation][3]][4]

[![python version][7]][8]  [![scikit version][11]][12] 

For this linear regression example, we will be using the heart disease dataset, which is a public health dataset that can be retrieved from [Kaggle](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset).

 ![title](https://images.unsplash.com/photo-1628348070889-cb656235b4eb?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80)
   
For this particular example, we will be only using two fields, the _trestbps_ (resting blood pressure in mm/hg) and _thalach_ (maximum heart rate achieved). There isn't much correlation between the data but for demonstration purposes, we will be using them to estimate linear regression using existing scikit libraries and also by using manual calculations in Python.

To calculate for the intercept or the _b_ in _y = mx + b_, we use the following formula:
* Intercept = [(ΣY)(ΣX2) – (ΣX)(ΣXY)] /  [n(ΣX2) – (ΣX)^2]

To calculate for the slope or the _m_ in _y = mx + b_, we use the following formula:
*  Slope = [n(ΣXY) – (ΣX)(ΣY)]  /  [n(ΣX2) – (ΣX)2]

We then compared our values to what is being calculated in sk-learn.

```python
import matplotlib.pyplot as plt
from scipy import stats

slope, intercept, r, p, std_err = stats.linregress(linear_table["X"], linear_table["Y"])
print(f"y = {slope}x + {intercept}")
```

[1]: https://img.shields.io/badge/donate-gcash-green
[2]: https://drive.google.com/file/d/1JeMx5_S7VBBT-3xO7mV9YOMfESeV3eKa/view

[3]: https://img.shields.io/badge/donate-paypal-blue
[4]: https://www.paypal.com/paypalme/mcabanlitph

[5]: https://img.shields.io/badge/license-GNUGPLv3-blue.svg
[6]: https://github.com/mcabanlit/heart-disease/blob/main/LICENSE.md

[7]: https://img.shields.io/badge/python-3.10-blue
[8]: https://www.python.org/

[9]: https://img.shields.io/badge/pywebio-1.6.1-dark
[10]: https://pywebio.readthedocs.io/en/latest/

[11]: https://img.shields.io/badge/scikit--learn-1.1.1-orange
[12]: https://scikit-learn.org

[13]: https://img.shields.io/badge/build-passing-green
[14]: https://heart-disease-pywebio.herokuapp.com/
