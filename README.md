# Ethnocentrism Inventory

An anonymous, single-page web version of the Generalized Ethnocentrism (GENE) Scale, built as an in-class activity for Introductory Psychology (Psych 100). Students answer 22 statements, get an automatically scored result with a plain-language interpretation written for first-year college students, and can optionally save their results as a PDF.

The whole thing is one file, `index.html`, with no dependencies, so it can be hosted for free on GitHub Pages or any static web host.

## The instrument

### What it measures

Ethnocentrism is the tendency to see your own culture as the center of the world and to judge other cultures by its standards. The GENE Scale was developed by James W. Neuliep and James C. McCroskey to measure ethnocentrism in a way that applies to anyone, regardless of their cultural background (as opposed to earlier scales written specifically for one country).

### Format

The revised scale has 22 statements rated on a five-point scale (1 = Strongly disagree, 5 = Strongly agree). Respondents are told to work quickly and record their first reaction.

### Scoring

Only 15 of the 22 items are scored. The scoring rules, following the authors' instructions, are:

| Step | Items | What to do |
|---|---|---|
| Reverse-score | 4, 7, 9 | Recode so 1 = 5, 2 = 4, 3 = 3, 4 = 2, 5 = 1 |
| Drop (filler items) | 3, 6, 12, 15, 16, 17, 19 | Not scored |
| Sum | 1, 2, 4, 5, 7, 8, 9, 10, 11, 13, 14, 18, 20, 21, 22 | Add the 15 remaining (recoded) responses |

Scores range from 15 to 75, and higher scores mean more ethnocentrism. Answering "Neutral" to every item gives 45. Neuliep's own self-assessment guidance treats scores above 55 as high ethnocentrism.

Note that some paper handouts of this scale include a "TOTAL" line that invites students to add all 22 responses. That doesn't match the authors' scoring. The web page uses the correct method and turns the difference into a short research-methods lesson: students see both their naive total and their real score, with an explanation of reverse-scored items, acquiescence bias, and filler items.

### Reliability and validity

The scale's authors and later researchers report good internal consistency, with Cronbach's alpha typically in the .80 to .92 range. Neuliep (2002) reports evidence for its reliability and validity. As with any short self-report measure, scores are influenced by social desirability and by which group a respondent pictures as "my culture."

### About the comparison data

There is no nationally representative U.S. norm for this scale. Most published data come from student convenience samples. Rather than invent a national average, the results page shows real reference points from published studies:

- About 37: the average for roughly 750 university students in a 2022 *Scientific Reports* study.
- About 35: the average for Israeli and Palestinian teens (around age 16) at baseline in a peace-building program registered on ClinicalTrials.gov.
- 45: the neutral midpoint.
- Above 55: the authors' threshold for high ethnocentrism.

The Low (15–34), Moderate (35–55), and High (56–75) zones shown on the results chart are rough guides for classroom discussion. Only the "above 55" cutoff comes from the scale's authors. If you have your own class data or better norms for your population, see "Adapting the page" below.

## Attribution

The scale items and scoring procedure are the work of their authors. Please cite them when you use this activity:

> Neuliep, J. W., & McCroskey, J. C. (1997). The development of a U.S. and generalized ethnocentrism scale. *Communication Research Reports, 14*, 385–398.

> Neuliep, J. W. (2002). Assessing the reliability and validity of the Generalized Ethnocentrism Scale. *Journal of Intercultural Communication Research, 31*, 201–215.

The scale and its scoring instructions are distributed on James McCroskey's measures page: <https://www.jamescmccroskey.com/measures/ethnocentrism_scale.htm>. If you plan to use the scale for research or publication rather than classroom reflection, check the current permissions with the source.

Other sources used on the results page:

- Comparison sample of university students: "A cross-cultural comparison of ethnocentrism and the intercultural willingness to communicate between two collectivistic cultures," *Scientific Reports* (2022). <https://www.nature.com/articles/s41598-022-21179-3>
- Comparison sample of teens: "Peace-Building Interventions for Israeli and Palestinian Youth," ClinicalTrials.gov NCT02122887. <https://clinicaltrials.gov/study/NCT02122887>
- Pettijohn, T. F., & Naples, G. M. (2009). Reducing ethnocentrism in U.S. college students by completing a cross-cultural psychology course.

The web page itself (layout, plain-language hints, interpretations, and code) was created for a Psych 100 course. See "License" below.

## Privacy

The page was built to be genuinely anonymous:

- No data leaves the student's device. There is no server, form submission, analytics, tracking, or third-party script.
- No external fonts or libraries are loaded, so not even the student's IP address is shared with a font or CDN provider. (GitHub Pages itself, like any web host, may keep standard server logs.)
- Nothing is stored. No cookies, localStorage, or databases are used, and answers disappear when the tab is closed or refreshed.
- The optional name field only appears on the student's own PDF and is never saved or sent.

If you adapt the page, keep this in mind before adding anything that loads from another site (fonts, analytics, embedded forms).

## Using it in your class

### Deploy your own copy on GitHub Pages

1. Fork this repository, or create a new public repository and upload `index.html` and this `README.md`.
2. In the repository, go to **Settings → Pages**.
3. Under **Build and deployment**, set the source to **Deploy from a branch**, pick `main` and `/ (root)`, and save.
4. After a minute or two, your page will be live at `https://<your-username>.github.io/<repository-name>/`.

You can also just open `index.html` directly in a browser or put it on any other static host (your LMS, a department server, Netlify, and so on).

### Running the activity

- Share the link or a QR code at the start of class. The inventory takes about five minutes.
- Remind students to keep one group in mind as "my culture" for the whole inventory. The page defines this, but saying it out loud helps.
- The results page ends with three discussion questions you can use for think-pair-share or a short writing prompt.
- Students who want a record can tap **Save results as PDF**. In the print dialog, they choose "Save as PDF" as the destination. On phones, they use Share or Print, then save to Files or Drive.

### Seeing your class's distribution (optional)

Because the page collects nothing, there is no class dashboard. If you want to show the class where scores fell, ask students to submit only their number through an anonymous poll (for example, a clicker question or an anonymous LMS survey) and display the histogram. This also makes a nice bridge to talking about distributions, means, and sampling, since your class is itself a convenience sample.

### Discussion connections

The results page links the inventory to in-group bias, the minimal group paradigm, social identity theory, cultural relativism, the contact hypothesis, self-report limitations, and social desirability bias. It works well alongside units on research methods, social psychology, or culture.

## Adapting the page

Everything lives in `index.html`. Open it in any text editor. The main things you might change:

| What | Where to find it |
|---|---|
| Course label ("Psych 100 \| In-class activity") | The `<p class="course">` line near the top of `<body>` |
| Intro text and definitions | The `<header class="intro">` section |
| Item wording and plain-language hints | The `ITEMS` array in the `<script>`; each item has `t` (text) and an optional `hint` |
| Which items are reversed or unscored | The `REVERSE` and `FILLER` arrays right below `ITEMS` |
| Score bands and interpretation text | The `band()` function and the `BAND_TEXT` object |
| Comparison reference points | The `How you compare` section inside `renderResults()` |
| Shaded "typical" range on the chart | The `typical` div in `renderResults()` (currently 34–37) |
| Psych 100 concept connections and discussion questions | The `Connect it to Psych 100` and `Think about it` sections in `renderResults()` |
| Colors | The CSS variables in `:root` at the top of the `<style>` block (with a separate dark-mode set) |
| Remove the optional name field | Delete the `nameField` label, input, and note in `renderResults()` |
| Sources in the footer | The `<footer>` section |

A few cautions when adapting:

- **Changing the wording of the scored items changes the instrument.** The plain-language hints were added under the items rather than rewriting them so that scores remain comparable to published research. If you do reword items, say so on the page and treat comparisons to published norms as approximate.
- **If you change which items are scored, update the score range.** The chart and the 15–75 range assume 15 scored items.
- **If you add comparison data, describe the sample honestly** (who, where, how many, and when), and avoid calling convenience samples "national."
- **Test printing after changes.** Print styles are in the `@media print` block at the end of the CSS.

### Accessibility notes

The page uses native radio buttons grouped in fieldsets with legends, so it works with keyboards and screen readers. It has visible focus outlines, respects reduced-motion settings, supports light and dark mode, and is responsive down to small phone screens. Unanswered items are flagged by number when a student tries to see results early.

## Limitations

This is a classroom reflection tool, not a diagnostic or clinical instrument, and a single score says nothing about whether someone is a good person. Self-report scores reflect what people say rather than how they act, are sensitive to social desirability (especially when answered in a classroom), and depend on which group the respondent pictured as "my culture." Please frame results for students in that spirit.

## License

The scale items and scoring procedure belong to their original authors (see "Attribution"). For the page's code and original text, add the license of your choice here, for example the MIT License for code and CC BY 4.0 for the written explanations, so other educators know how they may reuse and adapt it.
