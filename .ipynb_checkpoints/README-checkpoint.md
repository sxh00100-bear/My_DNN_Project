{\rtf1\ansi\ansicpg936\cocoartf2868
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 # \uc0\u55357 \u56960  My DNN Project: \u20174 \u21476 \u20856 \u28860 \u20025 \u21040 \u29616 \u20195 \u35270 \u35273 \
\
[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/)\
[![TensorFlow 2.x](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)](https://tensorflow.org/)\
\
\uc0\u36825 \u26159 \u25105 \u30340 \u28145 \u24230 \u23398 \u20064 \u36827 \u21270 \u20043 \u36335 \u12290 \u35760 \u24405 \u20102 \u20174 \u26368 \u22522 \u30784 \u30340 \u20840 \u36830 \u25509 \u32593 \u32476 \u65288 Dense\u65289 \u21040 \u22797 \u26434 \u30340 \u21367 \u31215 \u31070 \u32463 \u32593 \u32476 \u65288 CNN\u65289 \u30340 \u25506 \u32034 \u36807 \u31243 \u12290 \
\
---\
\
## \uc0\u55357 \u56517  \u23398 \u20064 \u36827 \u24230 \u22320 \u22270  (Roadmap)\
\
| \uc0\u31456 \u33410  | \u20869 \u23481 \u20027 \u39064  | \u29366 \u24577  | \u26680 \u24515 \u25104 \u26524  |\
| :--- | :--- | :---: | :--- |\
| **Ch 01-10** | \uc0\u26426 \u22120 \u23398 \u20064 \u22522 \u30784 \u19982  Keras \u20837 \u38376  | \u9989  | \u27888 \u22374 \u23612 \u20811 \u21495 \u12289 \u25151 \u20215 \u39044 \u27979 \u23454 \u25112  |\
| **Ch 11** | \uc0\u28145 \u24230 \u31070 \u32463 \u32593 \u32476 \u35757 \u32451 \u25216 \u24039  | \u9989  | Batch Normalization\u12289 LR Finder |\
| **Ch 14** | **\uc0\u28145 \u24230 \u35745 \u31639 \u26426 \u35270 \u35273  (CNN)** | \u55356 \u57303 \u65039  | **CIFAR-10 \u35782 \u21035  (\u24403 \u21069 \u25915 \u22362 \u28857 )** |\
\
---\
\
## \uc0\u55357 \u56620  \u26680 \u24515 \u23454 \u39564 \u23637 \u31034 \
\
### 1. CIFAR-10 \uc0\u38477 \u32500 \u25171 \u20987 \
* **\uc0\u23454 \u39564 \u25551 \u36848 **: \u27604 \u36739  20 \u23618 \u20840 \u36830 \u25509 \u32593 \u32476 \u19982  3 \u23618 \u21367 \u31215 \u31070 \u32463 \u32593 \u32476 \u30340 \u24615 \u33021 \u24046 \u24322 \u12290 \
* **\uc0\u20851 \u38190 \u32467 \u35770 **: \
    * \uc0\u21476 \u20856 \u32593 \u32476 \u20934 \u30830 \u29575 \u29942 \u39048 \u65306 **~47%** (\u26080 \u35770 \u24590 \u20040 \u21152 \u28145 \u37117 \u27809 \u29992 )\
    * CNN \uc0\u21021 \u35797 \u25112 \u26524 \u65306 **~70%+** (\u24341 \u20837 \u31354 \u38388 \u29305 \u24449 \u25235 \u21462 )\
\
### 2. CNN \uc0\u27169 \u22411 \u26550 \u26500  (Architecture)\
```python\
# \uc0\u26680 \u24515 \u32467 \u26500 \u24555 \u29031 \
model = keras.models.Sequential([\
    keras.layers.Conv2D(64, 3, activation="relu", padding="same"),\
    keras.layers.MaxPooling2D(2),\
    # ... \uc0\u26356 \u22810 \u32454 \u33410 \u35831 \u26597 \u30475 \u20195 \u30721 \u25991 \u20214 \
])}