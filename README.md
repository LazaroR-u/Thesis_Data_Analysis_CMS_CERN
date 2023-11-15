# Thesis_Data_Analysis_CMS_CERN
This repository contains the code used for the analysis of current data generated by the Resistive Plate Chambers (RPCs) of the Compact Muon Solenoid (CMS) experiment at CERN. This analysis is an integral part of my undergraduate physics thesis project, conducted at the Benemérita Universidad Autónoma de Puebla.


# 1_Comparison_Map_Functions_RPCs_CERN
In this notebook we implement the new map function to the current data and compare it with the Mapse mapping function. Here, we used only the Mapse mapping dataframe that includes 1050/1056 chambers.

# 2_Analysis_of_Label_Change_History_RPCs
Within this notebook, we initiate by crafting a new mapping dataframe sourced from the label change history file. Subsequently, we conduct a comparative analysis against the existing Mapse mapping dataframe.

Following this, we enhance the new mapping dataframe by appending suffixes to the duplicate DPIDs, enabling the mapping of both chamber names using our updated mapping function.

We then proceed to apply both map functions: the Mapse mapping function and our new mapping function to the currents data, facilitating a thorough comparative study between the two.

Lastly, we meticulously scrutinize the differences by **comparing the histograms** derived from these two sets of mapped current data.

# 3_New_Currents_Distributions_Analysis

This study builds upon the analysis conducted by Mapse Ferreira.

In our approach, we introduce the following enhancements:

Updated Mapping Dataframe: We have generated a new mapping dataframe from the RPC label change history data, incorporating information for 1056 chambers and their respective HV DPIDs. In contrast, the Mapse mapping dataframe comprises only 1050 chambers, leaving six chambers unaccounted for.

Enhanced Mapping Function: We have developed a new mapping function that takes into consideration both chamber names for duplicate DPIDs. In comparison, the Mapse mapping function only provides one chamber name for duplicate DPIDs. This improvement allows for a more comprehensive and accurate mapping of chamber data, specially, in the entries of the histograms for the Endcap region.
