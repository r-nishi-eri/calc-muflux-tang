This program calculates the flux of cosmic-ray muons at a given angle at a given overburden depth.

[1] HOW TO COMPILE

This program is written in C++. Please compile in the following way.

> g++ calc-muflux-tang.cpp -o calc-muflux-tang

[2] HOW TO EXECUTE

This program reads a table of muons' range in standard rock (standardrock.txt).
Please move the execuable in the same directory with standardrock.txt.

> ./calc-muflux-tang 100 0.1
0.000271954

The first argument is the amount of material traversed by muons (unit: meter water equivalent).
The second argument is the zenith angle in the unit of radian.
The output of the program is the muon flux after passing through the material 
with a given thickness (standard rock) in the unit of cm^{-2} sec^{-1} steradian^{-1}.

[3] REFERENCES

Muon energy spectrum model is taken from
Tang et al. (2006) https://arxiv.org/abs/hep-ph/0604078

Muon energy-range in standard rock is taken from
Groom et al. (2001) https://doi.org/10.1006/adnd.2001.0861
