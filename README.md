# ClassiFIRE
ClassiFIRE classifies remotely sensed fire detections as wildfire or prescribed (Rx) fire. 

Note: This workflow, ClassiFIRE, is an academic research tool and is not affiliated with or 
endorsed by any commercial entity.

Data access:

Remotely sensed fire detections for the Southeast are available from Southeast Firemap (SEFM): 
https://www.landscapepartnership.org/networks/working-lands-for-wildlife/wildland-fire/fire-mapping/regional-fire-mapping/se-firemap

MTBS (Monitoring Trends in Burn Severity) are at: mtbs.gov

Wildfire reports are available from the Fire Occurence Database v7 (FOD): 
https://doi.org/10.2737/RDS-2013-0009.7

Landfire Disturbance and Treatment Polygons Geodatabase (Landfire) is at: landfire.gov

The Southeastern US Prescribed Fire Permit Database (Permits) is available by request: https://doi.org/10.3390/fire6100372

Energy Release Component (ERC) data are available from gridMET: https://www.climatologylab.org/gridmet.html

We followed these steps:

1) SEFM processing- SEFM cleaning and filtering
2) SEFM event clustering- Grouping of detections into "events"
3) MTBS- Processing of MTBS and spatiotemporal comparisons with events
4) FOD- Processing of FOD and spatiotemporal comparisons with events
5) Landfire- Processing of Landfire and spatiotemporal comparisons with events
6) Permits- Processing of Permits and spatiotemporal comparisons with events
7) Post-matching- Application of data hierarchy, date calculations, ERC calculations
8) Random forest- We used spatiotemporally matched events to train/validate ClassiFIRE and applied to unmatched events.






