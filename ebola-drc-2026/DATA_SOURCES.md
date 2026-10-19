---
title: "Ebola DRC 2026 — data sources"
project: ebola-drc-2026
type: sources
generated_by: sources_list.py
updated: 2026-10-19 10:01 UTC
---

# Data sources — Ebola (Bundibugyo) DRC 2026

> Generated automatically from the dashboard's data files; lists only sources in current use. Interactive dashboard: [outbreak.loew-beer.at](https://outbreak.loew-beer.at). The May 2026 initial source scan is archived separately.

## Core data sources

| Source | Provides | How collected | Latest data | Status |
|---|---|---|---|---|
| [INSP situation reports via INRB-UMIE](https://github.com/INRB-UMIE/Ebola_DRC_2026) | National and health-zone confirmed cases, deaths, recoveries, suspected cases in isolation, PCR machine list, WorldPop population by zone. Primary source for all case series and charts. Notification dates, not onset dates. Code MIT; data reused with attribution. | Automatic, hourly (digitised INSP sitreps; INRB-UMIE build files). | 2026-10-16 | current |
| [CDC Ebola situation summary](https://www.cdc.gov/ebola/situation-summary/index.html) | Confirmed cases and deaths by country (DRC, Uganda, Kenya, France). Used for headline totals across countries and as a cross-check of INSP. | Automatic, hourly, through a public reader proxy (r.jina.ai) because CDC blocks server requests. | 2026-10-14 | current |
| [WHO Disease Outbreak News](https://www.who.int/emergencies/disease-outbreak-news) | Official situation updates: totals, provinces, contact follow-up, risk assessment. Ebola DONs in this outbreak: DON602, 603, 605, 606, 615–619 (DON604 is hantavirus, DON620 is not Ebola). | New DONs detected automatically (RSS); figures entered after review. | 2026-10-08 | current |
| [Africa CDC situation reports (Knowledge Hub)](https://khub.africacdc.org) | Contact follow-up (national and by province), treatment-centre bed occupancy, health-worker infections, province totals. Publication is irregular; see the data freshness table. | Automatic, hourly (PDF parsed). | 2026-10-02 | late |
| [Pathoplexus (ebola-bdbv)](https://pathoplexus.org/ebola-bdbv) | Counts of 2026 genomes by collection week, province and release delay. Most 2026 genomes are under restricted-use terms; no sequences or accessions are republished. | Automatic, hourly (LAPIS API, aggregates only). | 2026-10-17 | current |
| Curated humanitarian indicators | Displacement, food insecurity, orphans, collateral health impact, funding, access incidents. Figures older than 45 days are flagged on the dashboard. | By hand from published UN, NGO and peer-reviewed reports (each listed below). | 2026-10-06 | current |

## Latest documents used

- [Africa CDC Sitrep #132, October 2 2026](https://khub.africacdc.org/records/resource/bundibugyo-virus-disease-outbreak-situational-report-october-2-2026)
- [WHO DON616](https://www.who.int/emergencies/disease-outbreak-news/item/2026-DON616), 2026-08-28
- [WHO DON617](https://www.who.int/emergencies/disease-outbreak-news/item/2026-DON617), 2026-09-10
- [WHO DON618](https://www.who.int/emergencies/disease-outbreak-news/item/2026-DON618), 2026-09-25
- [WHO DON619](https://www.who.int/emergencies/disease-outbreak-news/item/2026-DON619), 2026-10-08
- Kenya cases: Kenya MoH via WHO AFRO (2026-10-16); WHO DON619

## Contact follow-up figures

Published snapshots only; definitions differ by source, so they are not joined into a trend.

| Date | Follow-up | Source | Definition |
|---|---|---|---|
| 2026-06-10 | 75.5% | Africa CDC Sitrep #24 | under follow-up / listed (DRC + Uganda) |
| 2026-08-10 | 83.5% | Africa CDC Sitrep #85 | under follow-up / listed (DRC + Uganda) |
| 2026-09-25 | 83.4% | [WHO DON618 (publication date)](https://www.who.int/emergencies/disease-outbreak-news/item/2026-DON618) | monitored / requiring follow-up |
| 2026-10-02 | 73.1% | [Africa CDC Sitrep #132](https://khub.africacdc.org/records/resource/bundibugyo-virus-disease-outbreak-situational-report-october-2-2026) | seen that day / due that day (DRC) |
| 2026-10-06 | 80.4% | [WHO DON619](https://www.who.int/emergencies/disease-outbreak-news/item/2026-DON619) | monitored / requiring follow-up |

## Humanitarian and response figures (curated; last reviewed 2026-10-18)

| Figure | Value | As of | Source |
|---|---|---|---|
| People displaced in Ituri | 1.1 million+ | 2026-09-28 | [UN News / OCHA](https://news.un.org/en/story/2026/09/1168465) |
| Displaced people in the five provinces with confirmed cases | 4.4 million | 2026-08-06 | [UN News / UNHCR](https://news.un.org/en/story/2026/08/1168092) |
| People in Ituri facing crisis-level hunger or worse | 1.7 million | 2026-10-06 | [WFP](https://www.wfp.org/stories/eastern-drc-ebola-outbreak-threatens-deepen-hunger-wfp-ramps-emergency-support) |
| Children orphaned or separated by Ebola | 1,900+ | 2026-09-28 | [UNICEF](https://www.unicef.org/press-releases/more-1900-children-orphaned-or-separated-their-families-ebola-eastern-dr-congo) |
| Drop in use of essential health services in hotspots | -42% | 2026-08-05 | [UNICEF](https://www.unicef.org/press-releases/dr-congo-ebola-child-deaths-pass-300-unicef-warns-outbreak-also-threatens-essential) |
| Drop in first-dose measles vaccination, Mongbwalu | -69% | 2026-08-05 | [UNICEF](https://www.unicef.org/press-releases/dr-congo-ebola-child-deaths-pass-300-unicef-warns-outbreak-also-threatens-essential) |
| Suspected measles cases nationally, Jan-Jul 2026 | 108,643 | 2026-07-19 | [MSF](https://www.doctorswithoutborders.org/latest/ebola-disease-response-continues-other-health-needs-dr-congo-must-not-be-neglected) |
| DRC humanitarian response plan funded | 48% | 2026-09-01 | [OCHA](https://www.unocha.org/publications/report/democratic-republic-congo/mr-tom-fletcher-under-secretary-general-humanitarian-affairs-and-emergency-relief-coordinator-virtual-briefing-member-states-ebola-outbreak-democratic-republic-congo-1-september-2026) |
| UNFPA Ebola appeal funded | 9% | 2026-10-01 | [UNFPA](https://ifp.nyu.edu/2026/grey-literature/unfpa-ebola-outbreak-democratic-republic-congo-appeal-june-november-2026/) |
| Insecurity restricts humanitarian access to Fataki, Drodro and Lita health zones; some aid organisations suspe | Ituri | 2026-10-01 | [UN News / OCHA](https://news.un.org/en/story/2026/10/1168499) |
| Ebola transit centre burned down in Kigonze displacement camp (about 19,000 people) after soldiers entered the | Ituri | 2026-09-30 | [UN News](https://news.un.org/en/story/2026/10/1168499) |
| More than 3,000 people fled Rhoe displacement camp (Djugu) after clashes intensified on 27 September. | Ituri | 2026-09-27 | [UN News / OCHA](https://news.un.org/en/story/2026/10/1168499) |
| Fighting in Masisi displaced more than 24,000 people since mid-September. | Nord-Kivu | 2026-09-15 | [UN News / OCHA](https://news.un.org/en/story/2026/10/1168499) |
| PARTNERS trial (MBP134, remdesivir) | Enrolling since 2026-07-02; no results published |  | [Science](https://www.science.org/content/article/first-ever-treatment-trial-ebola-bundibugyo-kicks-congo) |
| Ervebo ring-vaccination trial (cross-protection) | Phase 3, 70,000 doses made available; no efficacy results published. Evidence for cross-protection is limited |  | [Al Jazeera; medRxiv meta-analysis](https://www.aljazeera.com/news/2026/8/7/ebola-cases-top-4000-in-drc-as-who-urges-ervebo-vaccine-trial) |

## Reviewed literature and reports (23 approved)

Found by the twice-weekly scan (UN News, MSF, Europe PMC) and approved by a person before use.

- 2026-10-16: [WHO scales up Ebola readiness in 22 countries across three continents](https://news.un.org/feed/view/en/story/2026/10/1168613) — UN News
- 2026-10-15: [Children are being left behind in the Ebola disease response](https://www.msf.org/children-are-being-left-behind-ebola-disease-response) — MSF
- 2026-10-15: [WHO urges vigilance after Kenya confirms second Ebola case](https://news.un.org/feed/view/en/story/2026/10/1168602) — UN News
- 2026-10-14: [DR Congo: Cholera cases spike amid fight against Ebola](https://news.un.org/feed/view/en/story/2026/10/1168595) — UN News
- 2026-10-08: [Bundibugyo virus: coordinating a cross-border response](https://doi.org/10.1016/s0140-6736(26)01980-x) — Lancet (London, England)
- 2026-10-08: [Sixteen Days Undetected: Growth Dynamics and the Case for Pre-Positioned Response Capacity in the 2026 Bundibugyo Virus Disease Outbreak, Democratic Republic of the Congo](https://doi.org/10.1016/j.ijid.2026.109170) — International journal of infectious diseases : IJID : official publication of the International Society for Infectious Diseases
- 2026-10-08: [Ebola: Kenya marks first case and fatality in Bundibugyo strain outbreak](https://doi.org/10.1136/bmj-2026-101091) — BMJ (Clinical research ed.)
- 2026-10-08: [Filovirus reactive antibodies in wildlife hunting communities suggest ongoing zoonotic spillover in forested Guinea](https://doi.org/10.1038/s41467-026-77653-3) — Nature communications
- 2026-10-07: [Kenya races to trace all contacts after first Ebola death, WHO official says](https://news.un.org/feed/view/en/story/2026/10/1168542) — UN News
- 2026-10-06: [‘Ebola takes the people children depend on’: UNICEF](https://news.un.org/feed/view/en/story/2026/10/1168531) — UN News
- 2026-10-05: [Species Breadth Is a Preparedness Metric: Lessons from the 2026 Bundibugyo Virus Disease Outbreak](https://doi.org/10.1080/22221751.2026.2744490) — Emerging microbes & infections
- 2026-10-05: [Ebola disease outbreak spreads like a megafire in North Kivu](https://www.msf.org/ebola-disease-outbreak-spreads-megafire-north-kivu) — MSF
- 2026-10-01: [Early Action Review of Detection, Notification, and Response Timeliness during Cross-Border Bundibugyo Virus Disease Outbreak, Uganda, 2026](https://doi.org/10.3201/eid3210.261411) — Emerging infectious diseases
- 2026-10-01: [Bundibugyo virus disease and the unfinished countermeasure agenda](https://doi.org/10.2471/blt.26.296654) — Bulletin of the World Health Organization
- 2026-10-01: [In this month’s Bulletin](https://europepmc.org/article/PMC/PMC13626523) — Bulletin of the World Health Organization
- 2026-10-01: [MSF staff tests positive for Ebola disease and medically evacuated](https://www.msf.org/msf-staff-tests-positive-ebola-disease-and-medically-evacuated) — MSF
- 2026-10-01: [Ebola response faces setback as transit centre burns down in DR Congo camp](https://news.un.org/feed/view/en/story/2026/10/1168499) — UN News
- 2026-09-30: [What will it take to end the Ebola disease outbreak in DRC](https://www.msf.org/what-will-it-take-end-ebola-disease-outbreak-drc) — MSF
- 2026-09-29: [DRC: Early access to care and oxygen decisive for Ebola patients’ survival – WHO](https://news.un.org/feed/view/en/story/2026/09/1168481) — UN News
- 2026-09-29: [Security Council LIVE: DRC peace deals fail to halt fighting as Ebola deepens crisis](https://news.un.org/feed/view/en/story/2026/09/1168482) — UN News
- 2026-09-28: [How mistrust emerged in real time in the Bundibugyo virus disease outbreak: 'Ebola business', social media and the history of mistrust in Ebola epidemics in eastern Congo](https://doi.org/10.1136/bmjgh-2026-025522) — BMJ global health
- 2026-09-28: [DR Congo Ebola emergency: Calls grow for urgent humanitarian access](https://news.un.org/feed/view/en/story/2026/09/1168465) — UN News
- 2026-09-25: [From isolation to burial: dignity in the Bundibugyo virus disease response](https://doi.org/10.1016/s0140-6736(26)01905-7) — Lancet (London, England)

## Methods and reference values

- [Historical Bundibugyo fatality (pooled 2007 Uganda and 2012 DRC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC5124280/): Pooled 32.8% (25.8–40.2%); reference lines and the deaths-based ascertainment model.
- Rt method: Cori and colleagues, 2013 (EpiEstim): Instantaneous reproduction number from the INSP national series, 7-day window.
- Serial interval: mean 11.4 days, SD 5.0: Bundibugyo-specific value used by the Rt pipeline (attributed to MacNeil and colleagues, 2010).
- Onset-to-death delay: mean 11.4 days: McCabe and colleagues, 2026, Lancet Infectious Diseases; used to lag deaths in the ascertainment model.
- Rt-to-growth conversion: Wallinga and Lipsitch, 2007: Used for the 4-week projection (gamma serial interval).
- [Nextstrain ebola/bdbv](https://nextstrain.org/ebola/bdbv): Live phylogeny embedded on the Genomics tab.
- [WorldPop](https://www.worldpop.org): Modelled population for attack rates (via INRB-UMIE).
- [OpenStreetMap](https://www.openstreetmap.org): Map tiles.

## Not available publicly

- Case-level linelist (age, sex, onset, outcome)
- Share of new cases already on a contact list
- Testing cascade (samples collected, tested, positive, turnaround)
- Location below health-zone level
