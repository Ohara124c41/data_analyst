# Communicating Data Findings: Nuclear Reliance vs Reactor Fleets
### Christopher O'Hara, PhD, EngD

## Dataset
- Nuclear power plant locations and reactor counts (Kaggle): https://www.kaggle.com/datasets/liananapalkova/nuclear-power-plants  
- IAEA nuclear electricity statistics 2022 (Kaggle): https://www.kaggle.com/datasets/kanchana1990/nuclear-share-of-electricity-generation  

Why both: the plant dataset tells us where infrastructure sits (sites, reactors) while the IAEA data tells us how much electricity is actually supplied by nuclear. Merging on country lets us see whether fleet size aligns with reliance.

Wrangling: harmonized country names to uppercase, aggregated plant data to country-level counts/reactors, then left-joined the IAEA share data to relate reliance to fleets and regions.

## Summary of Findings
- Nuclear share is right-skewed (median ~18%); only a few countries exceed 50–60% reliance.
- Plant sites are concentrated in Western Europe and Northern America; other regions have sparse coverage.
- Reactor count correlates weakly with nuclear share (corr ~0.07); some countries achieve high share with modest fleets.
- Europe (Central/Eastern and Western) maintains high share even in low and mid-sized fleet bins; other regions only eclipse ~15% when fleets reach 6–10 reactors.
- Regional medians: Europe leads (~32–35%), Northern America moderate (~16%), others notably lower.

## Key Insights for Presentation
1) Fleet size alone does not explain nuclear reliance: mid-sized European fleets outperform larger fleets elsewhere in share %.  
2) Infrastructure is unevenly distributed: Western Europe and Northern America host most sites, leaving other regions with limited coverage.  
3) Most countries rely on nuclear for under 35% of electricity; a small tail of high-reliance nations shapes the upper end.

Design notes: consistent region color encoding across plots; linear scales with clear labels; modest marker sizes to avoid overplotting given the small country sample.
