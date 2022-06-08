# Lookingglass-Creek-spring-Chinook-RRS
This repository provides the scripts used to generate individual reproductive success estimates for hatchery-origin (HOR) and natural-origin (NOR) spring Chinook salmon that spawned in Lookingglass Creek, OR from 2008-2016.

These analyses are detailed in the manuscript *Improved productivity of naturalized spring Chinook salmon following reintroduction from a hatchery stock in Lookingglass Creek, Oregon*, which has been submitted for review. 

## Data Ownership
To conform with data sharing practices followed by the data owners, the Confederated Tribes of the Umatilla Indian Reservation (CTUIR) & the Oregon Department of Fish and Wildlife (ODFW), and to honor principles of Indigenous Data Sovereignty, the raw data files are not available in this repository. If you would like access to these data so that you may execute the scripts with that dataset, please contact the following: Hayley Nuetzel at hnuetzel@critfc.org, Gene Shippentower at geneshippentower@ctuir.org, Les Naylor at lesnaylor@ctuir.org, and Carrie Crump at carriecrump@ctuir.org. 

## Repository Description
In addition to the files included here, you'll need to make sure you have SNPPIT and COLONY2 downloaded to your machine. Also please take note of file paths, as you'll likely need to edit those within the Rmarkdown files according to how you structure your Rproject. 

The Rmarkdown files are numbered according to the order in which I performed the various analytical steps that eventually culminated in the input file for the GLM analyses. The necessary data files can be accessed upon request (see above), and the functions within the IDFGEN package should be accessible within the zipped IDFGEN package. Lastly, the LKG_RRS_ParentCollections.xlsx file outlines how I structured each parentage run, such that a single Offspring Collection, which was the combination of the Offspring Life Stage and Collection Year (e.g., Adult_2012), was run against a group of potential parents (outlined in the Potential Parent Collections) column. Each Offspring Collection was run individually in SNPPIT and COLONY2. 

I performed this set of analyses ~3-4 different times, because as is often the case with parentage analyses, the preliminary runs highlight potentially missed collections or ways in which the analysis could be improved. While the individual assignments would shift slightly between these analytical attempts, the inference always remained the same - NOR fish consistently displayed higher reproductive success (RS). For this reason, I'm certain your reproduction of these analyses will yield some slightly different assignments. I am even more certain of this because there are steps (particularly Step 8) where you must look at the excel files with your own eyes and identify assignments that should be included in the RS estimations. In the end, I tried to automate as much in R scripts that was possible, but at some point, you still really need to look at the data. 

Please don't hesitate to reach out with questions/suggestions for analytical improvement for future analyses! 

Thank you for reading! 
