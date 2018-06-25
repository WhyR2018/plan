# strideter: R package for identifying individual's steps from sub-second level accelerometry data of walking

[Marta	Karas,	Johns Hopkins University, Bloomberg School of Public Health]()

## Description

Wearable accelerometers can provide objective high-density measurements of human physical activity through recording movement acceleration. Recent advances in technology and the decreasing cost of wearable devices led to an explosion in the popularity of wearable technology in health research. For example, quantifying gait parameters has become increasingly important for epidemiological and clinical studies. Due to complexity and volume of accelerometry data, automatic and unsupervised methods for precise walking segmentation are needed. 

The R strideter package implements method we propose to precisely identify beginnings and ends of individual's steps from sub-second level accelerometry data of walking. The method employs the continuous dictionary learning framework to identify strides (two subsequent steps) from accelerometry data.  Precisely, we define data-derived baseline patterns, which we name as movelets, representing a population-specific stride. Next, we perform two-step strides segmentation by combining pattern-recognition with a maxima-detection approach to precisely identify beginnings and ends of individual's strides. 

We demonstrate the proposed method using accelerometry data collected during 450-meter outdoor walk of 32 study participants wearing accelerometers on a wrist, hip and both ankles. We validate the performance of the method and discuss individual-specific gait characteristics.