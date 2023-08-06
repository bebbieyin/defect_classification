# Defect Classification in Factory with XGBoost

## Introduction

This project aims to classify whether an item in a factory's production line is considered as a defect. The notebook contains thoughts and processes througout the project. Including the feature engineering, data understanding, motivations behind the methods used, handling the imbalanced class problem. 


## Dataset Description
- Example of Product Name : I-B-XA1207672-190701-00494.
- ID = PROX TRAZ = it's a unique code given to the product.
- XA1207672 is the reference.
- 190701 is the date: here 01st of July of year 2019.
- 00494 is the unique code given to the product, whatever it happens, the product will have this id number frozen forever.
- This number is increased by 1 each time we process a new product, every 12s. So for example : I-B-XA1207672-190701-00495 is the next product.
- Inputs : Input features are measures collected on dierent assembly stations with the sensors or devices connected to Programmable Logic Controllers which are storing all of them to keep the full quality traceability (Examples : OP070 V 1 angle value, OP120 Rodage I value, etc. . . ).
- Output : This is the result value of OP130 (test bench). Value 0 is assigned to OK samples (passed) and value 1 is assigned to KO samples (failed). This is the combined result of multiple electrical, acoustic and vibro-acoustic tests.