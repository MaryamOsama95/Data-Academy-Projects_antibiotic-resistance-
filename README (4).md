# Antibiotic Resistance Patterns of Cultured Uropathogens in Primary Health Care, Muscat Governorate

> Which uropathogens are most common among urinary tract infection (UTI) cases that did not respond to the first antibiotic course in primary health care in Muscat, and how do antibiotic results relate to gender, age, comorbidities and location?

## Background
Urinary tract infections are among the most common bacterial infections in primary care, and most are treated empirically before culture results are available. Rising antibiotic resistance makes local surveillance important, yet most studies in Oman come from secondary and tertiary hospitals, with only a few at the primary care level. This project describes resistant UTI cases across six wilayats of Muscat governorate and tests which antibiotic results are associated with patient characteristics.

## Data
- Retrospective data from laboratories in six wilayats: Mutrah, Bausher, Muscat, Seeb, Amerat and Qurayyat.
- **3,837** positive urine cultures were received; **525** cases that did not respond to the first antibiotic course were analysed (2018-2022).
- Variables: gender, age, wilayat, comorbidities (DM, HTN, thyroid, recurrent UTI, pregnancy, renal disease / kidney stones, CNS / spinal disease, bedridden / catheter, DLP), symptoms, recent antibiotic use, previous positive culture, sample year, isolated pathogen, and results for 20 antibiotics.
- Patient-level data is **not included** in this repository because it contains patient identifiers.

## Methodology
1. Descriptive statistics and charts for the resistant group (frequencies, percentages, mean and SD for age).
2. Focus on the two most common pathogens: *Escherichia coli* and *Klebsiella pneumoniae*.
3. Pearson Chi-square and Fisher's exact tests (95% confidence level) between each antibiotic result and gender, age group (<=30, 30-60, >=60), DM, HTN, pregnancy, and renal disease / kidney stones, and by wilayat.
4. Cramér's V to measure the association between each antibiotic and previous positive culture.

## Results

**Sample description (n = 525)**

| Characteristic | Result |
|---|---|
| Age | mean 48.9 years (SD 20.3), range 12-104 |
| Gender | 83.6% female, 16.4% male |
| Previous positive culture | 82.1% no, 17.9% yes |
| Symptoms | lower urinary tract 54.1%, mixed 7.8%, asymptomatic 7.6%, upper urinary tract 3.6%, not recorded 26.9% |
| Sample year | 2018: 110, 2019: 104, 2020: 110, 2021: 98, 2022: 103 |

**Pathogens:** *E. coli* 64.8%, *Klebsiella pneumoniae* 10.7%, coliform bacteria 5.5%, *Streptococcus agalactiae* 3.2%, *Staphylococcus aureus* 3.2%, all others 2.5% or less.

**By wilayat**

| Wilayat | Positive cultures | Resistant cases | Resistant / positive |
|---|---|---|---|
| Mutrah | 369 | 106 | 28.7% |
| Bausher | 976 | 100 | 10.2% |
| Muscat | 832 | 60 | 7.2% |
| Seeb | 393 | 31 | 7.9% |
| Amerat | 562 | 140 | 24.9% |
| Qurayyat | 705 | 88 | 12.5% |
| **Total** | **3,837** | **525** | **13.7%** |

**Statistically significant associations (Chi-square / Fisher, p < 0.05)**

| Factor | *E. coli* | *K. pneumoniae* |
|---|---|---|
| Gender | Gentamicin | None |
| Age group | Cefotaxime, ciprofloxacin, cefuroxime | Piperacillin-tazobactam |
| DM | Cefuroxime (parenteral), cefazolin, ceftazidime, cefotaxime, cefuroxime | Ciprofloxacin |
| HTN | Cefuroxime (parenteral), cefotaxime | Amoxicillin-clavulanate, cefuroxime |
| Pregnancy | None | None |
| Renal disease / kidney stones | None | Trimethoprim-sulfamethoxazole, amoxicillin-clavulanate, ciprofloxacin, cefuroxime, gentamicin |

**Previous positive culture (Cramér's V):** for *E. coli*, nitrofurantoin, amoxicillin-clavulanate and nalidixate were the least associated with previous positive cultures; for *K. pneumoniae* only amoxicillin-clavulanate was significantly associated.

## Limitations
- The dataset contains only cases that did not respond to the first antibiotic course, so there is no comparison group. Differences by gender or age therefore describe this group and do not show which patients are more likely to develop resistance (for example, women are generally over-represented among UTI patients).
- Many tests were run (about 20 antibiotics across several factors and two pathogens) without multiple-testing correction, so some significant results may be chance findings.
- Several cells have small counts, and symptoms were not recorded for 26.9% of cases.
- Retrospective laboratory data from selected centres, so results may not generalise to all of Oman.

## Repository structure
```
├── README.md
├── Antibiotic_resistance_report.pdf     # full report
└── images/                              # charts used in the report
```

## Tools
- IBM SPSS Statistics
- Microsoft Word
