# 2019 Clayton Griffin Over Current Relay Student Paper Competition Repository

This repository contains the over current relay models used in the following paper submitted for the 2019 Clayton Griffin student paper award competition.

## How to simulate it?
Follow the steps below:

- Download the relaymodel.mo package found [here](https://github.com/ALSETLab/2019_Clayton_Griffin_OverCurrentRelay/tree/master/Model).
- Load the package onto a Modelica Compliant software
- Open the package 


### Cross Verification
Open the model run and `./Test/TestRecordOverCurrentRelay` This consists of 3 simulations, for each of the different relay types the 3 parameters must be set. The parameter window of the relay model should be filled like this:
![paramters](https://github.com/ALSETLab/2019_Clayton_Griffin_OverCurrentRelay/blob/master/Figures/parameters.png). 
  - For Standard Inverse Relay, set the following parameters:
    - standardInverseData.alpha.alpha
    - standardInverseData.c.C
    - standardInverseData.eps.eps
  - For Very Inverse Relay:
    - veryInverseData.alpha.alpha
    - veryInverseData.c.C
    - veryInverseData.eps.eps
  - For Extremely Inverse Relay:
    - extremelyInverseData.alpha.alpha
    - extremelyInverseData.c.C
    - extremelyInverseData.eps.eps
 

### Application Example
Open the model and run `./Test/TestFaultMSL`. This consists of 3 simulations, for each of the different relay types the 3 parameters must be set:
 - For Standard Inverse Relay, set the following parameters:
    - standardInverseData.alpha.alpha
    - standardInverseData.c.C
    - standardInverseData.eps.eps
  - For Very Inverse Relay:
    - veryInverseData.alpha.alpha
    - veryInverseData.c.C
    - veryInverseData.eps.eps
  - For Extremely Inverse Relay:
    - extremelyInverseData.alpha.alpha
    - extremelyInverseData.c.C
    - extremelyInverseData.eps.eps
  
## Additional Information

The following information may be also be useful:
- The original final version for the paper is available [here](https://github.com/ALSETLab/2019_Clayton_Griffin_OverCurrentRelay/blob/master/Paper/SubmissionManuelNavarroCatalan.pdf).
- For cross verification purposes, the model for which this model was cross verified, can be found [here](https://ieeexplore.ieee.org/abstract/document/6389585).
-Depending on the set up, k may have to be modified to the tolerance found in `./RecordOverCurrentRelay/CalculationOperationTime` for cross verification and `./ElectricSystemOverCurrentRelay/CalculationOperationTime` for the application example


