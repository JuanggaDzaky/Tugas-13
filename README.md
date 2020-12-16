# Tugas-13

In [1]:
#program utama
d = int(input("Tinggi Tower adalah: 80 "))
fc = int(input("Tinggi User adalah:1,5 "))
area = input("Jumlah User adalah: 200 ")
ht = int(input("Jarak 200-700 meter adalah: "))

Tinggi Tower adalah: 80
Tinggi User adalah: 1,5
Jumlah user adalah: urban
Jarak 20-700 meter adalah: 200


In [2]:
import numpy as np

In [3]:
NtL = lambda x: 10*np.log10(x)

In [4]:
LtN = lambda x: 10**(x/10)

In [5]:
def rumusc1 (z):
  if z in range (400,1500):
    return 69.55

  elif z in range (1500,2000):
    return 46.3

In [6]:
def rumusc2 (z):
  if z in range (400,1500):
    return 26.16

  elif z in range (1500,2000):
    return 33.9

In [7]:
def rumuscm (area,fc):
  if area ==  "urban":
    return 0
  if area == "suburban":
    return -2*(np.log10(fc/28)**2 - 5.4)
  if area == "open":
    return -4.78*(np.log10(fc))**2 + 18.33*np.log10(fc) - 40.94
