Tracked line-by-line edits for `tex/intro.tex`

Note: line numbers refer to logical blocks/paragraphs rather than absolute file line numbers to keep edits robust against minor reflow.

1) File header / chapter opening (replace)
- Problem: Wordy and slightly inaccurate opening sentence. Minor grammar issues.
- Original (first paragraph):
  "The Planck experiment provides evidence that 68\% of our universe comprises dark energy, 27\% is dark matter and 5\% is baryonic matter \cite{10.1051/0004-6361/201321591}. The existence of dark matter is supported by multiple astronomical observations including galaxy rotation curves and gravitational lensing in the Bullet Cluster, where two colliding galaxy clusters exhibit clear separation between their mass and baryonic components \cite{10.1046/j.1365-8711.2000.03075.x}. Despite the observational evidence, the nature of dark matter and its interactions with ordinary matter remain poorly understood."
- Replacement (suggested):
  "Observations from the Planck satellite indicate that ordinary baryonic matter contributes roughly 5% of the Universe's energy density, while dark matter contributes approximately 27% and dark energy dominates the remainder \cite{10.1051/0004-6361/201321591}. Although the gravitational effects of dark matter are well established — from galaxy rotation curves to gravitational lensing such as that observed in the Bullet Cluster \cite{10.1046/j.1365-8711.2000.03075.x} — its particle nature and non-gravitational interactions remain unknown."
- Rationale: tighter, more formal phrasing; keeps references and motivation but is more precise.

2) Paragraph about WIMPs & candidates
- Problem: Long list of candidates, punctuation/spacing issues.
- Edits: Change "right-handed sneutrinos, and right-handed neutrinos in extra dimension theories" to "right-handed sneutrinos and Kaluza–Klein or right-handed neutrino candidates in extra-dimension models" (clarify phrase). Ensure citations follow punctuation.

3) Section "Indirect Dark Matter Searches" first paragraph
- Problem: Overlong sentences; inconsistent punctuation; awkward phrase "Dark matter interaction induced cosmic-ray (CRs) antideuterons and antihelium nuclei fluxes predicted by many different models exceed the estimated astrophysical background in the energy range of GeV or sub-GeV by orders of magnitude"
- Suggested rewrite snippet: "Many dark-matter models predict antideuteron and antihelium fluxes that exceed expected astrophysical backgrounds in the sub-GeV/n energy range by one or more orders of magnitude \cite{...}. This makes low-energy antinuclei an attractive channel for indirect searches."

4) Fokker–Planck equation paragraph
- Problem: Long run-on sentence that mixes description and equation; reformat.
- Edits:
  - Move definitions of symbols to a short, bulleted list under the equation, or to a single compact parenthetical sentence following the equation.
  - Example: after the equation, add: "Here, \psi(r,p,t) is..., Q(r,p) is..., D_{xx} is..., V is..., D_{pp} is..., and \tau accounts for..." Replace existing long sentence with that.

5) Sentence: "From the sub $GeV/n$ energy range, we will be able to detect rare antideuteron or antihelium3 events whose fluxes are two orders of magnitude higher than the background, providing us with background-free signatures. section.~\ref{chap:intro:IDMS:antideuteron} and section.~\ref{chap:intro:IDMS:antihelium} will introduce more about how to project primary flux from \ac{DM} interaction."
- Problems: Grammar, punctuation, and cross-reference style (lowercase "section.~" inconsistent).
- Suggested: "In the sub-GeV/n energy range, several models predict antideuteron and antihelium-3 fluxes that exceed astrophysical backgrounds by up to two orders of magnitude, yielding effectively background-free detection windows (see Figs.~\ref{fig:antideuteron_sensitivity}–\ref{fig:antihelium3_sensitivity}). Sections~\ref{chap:intro:IDMS:antideuteron} and \ref{chap:intro:IDMS:antihelium} explain how primary fluxes are modeled from dark-matter interactions."

6) Subsection on coalescence model (equation label consistency)
- Problem: Label `equ:antideutron_spectrum` is misspelled (antideutron vs antideuteron) and variable naming inconsistent (\textbf{$\bar{n}$}).
- Edits: Rename label to `equ:antideuteron_spectrum`. Replace boldface `\textbf{$\bar{n}$}` with plain `\bar{n}`. Ensure variables in text match equation symbols and that \gamma symbols are explained once.

7) Figures and captions
- Problem: Some captions contain narrative or repeated information; keep captions concise and descriptive.
- Edits: For `fig:antideuteron_sensitivity`, change caption to: "Predicted antideuteron fluxes and experimental sensitivities in the sub-GeV/n range. Signals from representative dark-matter models exceed the secondary background at low energies."

8) Section "Cosmic-ray antiprotons"
- Problems: Grammar and typos: "Cosmic antiprotons has being measured"; missing references formatting.
- Edits: "Cosmic-ray antiprotons have been measured by AMS and BESS, revealing features that remain puzzling and may be partially consistent with dark-matter annihilation or astrophysical sources \cite{...}."
- Equation formatting: label the equation and clarify variables: what is N_{\bar{p}}, x_R, and p_t?

9) Balloon experiments section
- Problems: Some sentences are verbose and contain grammatical errors. Replace colloquial constructions: "As a multi-decades form of scientific project" → "As a multi-decade scientific program".
- Tighten bullet list: remove capitalization errors and ensure NRC-style parallelism (all bullets start with verb forms or nouns consistently).

10) GAPS / GRAMS subsections
- Problems: Several tense and grammar inconsistencies and first-person phrasing: "I’m in charge of..." — convert to formal past-tense and limit first-person to a single "Contributions" paragraph.
- Edits: Change to: "I designed and tested the detector system for pGRAMS, including TPC and charge readout, and coordinated the pGRAMS launch schedule." Move personal role details to a new subsection "Author's contributions" or to the thesis preface/acknowledgements if appropriate.

11) Miscellaneous fixes
- Acronym expansions: ensure each \ac{...} is expanded at first occurrence in the file.
- Remove duplicate words (e.g., "would would") and fix plural/singular mismatches ("the \\ac{CRs} shower could be controlled" → "the CR shower can be reduced").
- Standardize units: use consistent spacing `GeV/n` and `km` and consistent math-mode for units when needed.

12) Add explicit "Thesis contributions" and "Thesis organization" paragraphs
- Insert after the opening background. Example contributions block (short bullets):
  - Flux modeling and propagation uncertainties for antideuteron and antihelium signals.
  - Instrument design, calibration, and balloon qualification for pGRAMS/pGAPS detectors.
  - Data analysis pipelines and sensitivity estimates for sub-GeV/n antinuclei searches.

13) Final polish
- Run a pass for grammar and style (I can apply a patch with these changes if you want).

Would you like me to apply these edits directly to `tex/intro.tex` as a patch, or would you prefer I produce a cleaned replacement file `tex/intro_clean.tex` and leave the original unchanged? I can also open a PR-style patch with hunks if you prefer line-by-line diffs.
