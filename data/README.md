## European Social Survey - Round 11 (ESS11.csv)

Round 11, on top of the base questionnaire, includes additional items on the themes *Social inequalities in health* (previously in round 7), *Climate change* (previously in round 8) and *Gender* (new theme). For further information on the variables included, you can consult the [codebook (Appendix A7)](https://ess.sikt.no/en/study/412db4fe-c77a-4e98-8ea4-6c19007f551b/).



## World Bank Data

World Development Indicators (WDI) is the primary World Bank collection of development indicators, compiled from officially recognized international sources. The `WDI` package allows you to search and download data from over 40 datasets hosted by the World Bank directly from within `R`, including the WDI. To do so, simply install and load the `WDI` package.

```
install.packages("WDI")

library(WDI)
```

You can search for data using keywords, e.g. GDP to look for indicators of Gross Domestic Product:
```
WDIsearch('gdp')
```
The keyword search relies on the `grep()` function. It is not case sensitive and supports [*regular expressions*](https://cran.r-project.org/web/packages/stringr/vignettes/regular-expressions.html). 



## KOF Globalisation Index (KOFGI\_2024\_public.dta)

The KOF Globalisation Index measures the economic, social and political dimensions of globalisation. More information, including a [codebook](https://ethz.ch/content/dam/ethz/special-interest/dual/kof-dam/documents/Globalization/2024/KOFGI_website_structure_variables.pdf), can be found on the [KOF website](https://kof.ethz.ch/en/forecasts-and-indicators/indicators/kof-globalisation-index.html).



## Populism and Political Parties Expert Survey (POPPA, party\_means.dta)

The POPPA data comprises an Expert Survey on European parties' positions on a number of different ideological dimensions, with a focus on measuring a party's populism. For further information on the variables included, you can consult the [codebook online](https://poppa-data.eu/wp-content/uploads/2024/11/codebook.html).



## ParlGov (parlgov\_election.csv)

ParlGov has collected data on a variety of countries, their elections, their outcome and the resulting cabinets. Generally, they provide an expansive data collection on elections and their results.



---

## References 

- European Social Survey European Research Infrastructure (ESS ERIC). (2025). _ESS11 - integrated file, edition 3.0 [Data set]_. Sikt - Norwegian Agency for Shared Services in Education and Research. <https://doi.org/10.21338/ess11e03_0>.

- Gygli, S., F. Haelg, N. Potrafke and J. Sturm. (2019). The KOF Globalisation Index – Revisited. _Review of International Organizations 14_ (3): 543-574. <https://doi.org/10.1007/s11558-019-09344-2>.

- Dreher, A. (2006). Does Globalization Affect Growth? Evidence from a new Index of Globalization. _Applied Economics 38_, 10: 1091-1110.

- World Bank. (2025). _World Development Indicators, July 2025_. World Bank Group. <https://databank.worldbank.org/source/world-development-indicators>.

- Arel-Bundock, V. (2025). _WDI: World Development Indicators and Other World Bank Data. R package version 2.7.9_. <https://vincentarelbundock.github.io/WDI/>.

- Zaslove, A., M. J. Meijers and R. A. Huber. (2025). The state of populism: Introducing the 2023 wave of the Populism and political parties expert survey. _Party Politics_ (OnlineFirst): 1-18. <https://doi.org/10.1177/135406882513618>.

- Döring, H., and P. Manow. (2024). _ParlGov 2024 Release_. <https://doi.org/10.7910/DVN/2VZ5ZC>.

