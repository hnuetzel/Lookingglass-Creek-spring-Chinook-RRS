# Lookingglass-Creek-spring-Chinook-RRS
This repository provides the scripts and data files used to generate individual reproductive success estimates for hatchery-origin (HOR) and natural-origin (NOR) spring Chinook salmon that spawned in Lookingglass Creek, OR from 2008-2016.

## Data Ownership
If you intend to use any part of this data set for analyses beyond reproduction of the parentage analyses outlined within this repository, you MUST receive permission from the entites that own the data. This includes the Confederated Tribes of the Umatilla Indian Reservation (CTUIR) and the Oregon Department of Fish & Wildlife (ODFW). Please contact Les Naylor at LesNaylor@ctuir.org to discuss permissions to use these data. 

## Repository Description
In addition to the files included here, you'll need to make sure you have SNPPIT and COLONY2 downloaded to your machine. Also please take note of file paths, as you'll likely need to edit those within the Rmarkdown files according to how you structure your Rproject. 

The Rmarkdown files are numbered according to the order in which I performed the various analytical steps that eventually culiminated in the input file for the GLM analyses. The necessary starter files are within the zipped "StarterFiles" folder, and the functions within the IDFGEN package should be accessible within the zipped IDFGEN package. Lastly, the LKG_RRS_ParentCollections.xlsx file outlines how I structured each parentage run, such that a single Offspring Collection, which was the combination of the Offpspring Life Stage and Collection Year (e.g., Adult_2012), was run against a group of potential parents (outlined in the Potential Parent Collections) column. Each Offspring Collection was run individually in SNPPIT and COLONY2. 

I performed this set of analyses ~3-4 different times, because as is often the case with parentage analyses, the preliminary runs highlight potentially missed collections or ways in which the analysis could be improved. While the individual assignments would shift slightly between these analytical attempts, the inference always remained the same - NOR fish consistently displayed higher reproductive success (RS). For this reason, I'm certain your reproduction of these analyses will yield some slightly different assignments. I am even more certain of this because there are steps (particularly Step 8) where you must look at the excel files with your own eyes and identify assignments that should be included in the RS estimations. In the end, I tried to automate as much in R scripts that was possible, but at some point, you still really need to look at the data. 

Please don't hestiate to reach out with questions/suggestions for analytical improvement for future analyses! 

Thank you for reading! 
