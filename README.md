# Sex and Gender Disparities in Mental Health: What Are Our Policies Doing?

An interactive dashboard reviewing whether national mental health policies
**acknowledge** differences by sex, gender and sexual orientation, and whether
they **act** on them.

**Live dashboard:** https://asarforindia.github.io/mental-health-gender-policy/

## Why this matters

Mental health conditions, neurological conditions, substance use and self-harm
(together, **MNSS**) affect people differently by sex, gender and sexual
orientation (together, **SGO**). Depression, for example, is more common in
women than in men. Yet research and policy rarely look beyond biological sex.
Recognising these differences is not enough on its own: policies also need
concrete actions to address them.

This dashboard asks two questions of each country's national documents:

1. **Say:** does any document acknowledge an SGO difference in mental health
   needs?
2. **Do:** does any document set out a concrete action to address one?

## The data at a glance

- **630 documents** across **125 countries**, screened in English from
  [WHO MiNDbank](https://www.mindbank.info/).
- Document types: national mental health policies, strategies, plans,
  legislation and WHO country reports.
- Documents by topic:

  | Topic | Documents |
  |---|---:|
  | Mental disorders | 396 |
  | Substance use | 154 |
  | Neurological / developmental | 43 |
  | Self-harm | 37 |

- Countries by WHO region: Europe 29, Western Pacific 26, Americas 22,
  Africa 21, Eastern Mediterranean 17, South-East Asia 10.

## What the dashboard shows

### 1. Say versus do

Each country is placed in one of six groups, based on all its documents taken
together:

| Group | Meaning | Countries |
|---|---|---:|
| Mentions sex differences and acts | A sex difference is named, and a document sets out a concrete action | 46 |
| Mentions sex differences, no action | A sex difference is named, but no document acts on it | 36 |
| Mentions gender or orientation and acts | Goes beyond sex to gender identity or orientation, with a concrete action | 14 |
| Mentions gender or orientation, no action | Names gender or orientation, but no document acts on it | 1 |
| Acts, but never says why | Has a sex-specific provision (e.g. separate wards for women), but no document states a difference in needs | 9 |
| Says nothing | No document mentions any difference or sets out an action | 19 |

A stacked bar and a world map show the groups. Click a group to list its
countries. Circles on the map show how many documents each country has, and
also mark small island states.

### 2. Sex, gender, orientation and action, mapped separately

Four small maps, one each for *mentions sex*, *mentions gender*, *mentions
orientation* and *concrete action*. Two controls apply to all four:

- **Show:** *Any document* (yes/no per country) or *% of documents* (shaded by
  share).
- **Topic:** All, Mental disorders, Neurological, Substance use, Self-harm.

### 3. By region and income

Bar charts of the share of countries meeting a chosen measure, broken down by
**WHO region** and by **World Bank income group** (Low, Lower-middle,
Upper-middle, High). They follow the topic chosen above.

### 4. Country profiles

Click any country, on a map or in a group list, to open a side panel with:

- its region, income group and say-versus-do group;
- counts of documents mentioning sex, gender and orientation, and with an
  action;
- every screened document, tagged Yes/No on each measure, with a short quote
  from the document where one was recorded.

## Definitions

- **Mentions:** at least one document notes a difference in mental health
  needs by sex, gender or orientation.
- **Concrete action:** at least one document has a policy, plan or legal
  provision addressing such a difference.
- **Quotes** in country profiles are the first passage recorded by the
  screeners, shortened.
- **Grey land** on the maps is outside the dataset.

## Limitations

- Only **national** documents are included. Subnational policies are not.
- Only documents available **in English** were screened. Documents published
  only in local languages are excluded, which under-represents some regions.
- Groups are based on what documents **say**, not on whether policies were
  implemented.

## Source and credit

Dataset: Dubey, Vuddemarry, Shrinivas, Rao et al., *"Dataset for Attention to
and Acknowledgement of Health Needs"*. Documents sourced from WHO MiNDbank.

## Viewing locally

The dashboard is a single self-contained HTML file (`index.html`) with all
data embedded. Only fonts load from Google Fonts. To view it:

```bash
# open directly
open index.html

# or serve it
python3 -m http.server 8000   # then visit http://localhost:8000
```

It works on desktop and mobile, and follows the system light/dark theme.

## Repository contents

| File | Purpose |
|---|---|
| `index.html` | The dashboard: markup, styles, script, map shapes and data in one file |
| `README.md` | This file |
