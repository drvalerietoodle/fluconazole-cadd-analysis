# Fluconazole: When the Structure Doesn’t Match the Biology

**Dr. Valerie Toodle**

**Tools:** Python, RDKit, Pandas, Matplotlib  
**Focus:** Computational drug analysis, molecular descriptors, CADD

---

## Why I Did This

Fluconazole is a well-known antifungal. Structurally, it’s not designed to act in the brain.

But in my own work, I’ve seen evidence suggesting potential neuroprotective effects. (This work builds on findings from my published research:
Toodle, V. et al. (2022). "Fluconazole Is Neuroprotective via Interactions with the IGF-1 Receptor." Neurotherapeutics. DOI: 10.1007/s13311-022-01265-0)

That raised a simple question:

> Does fluconazole’s structure actually support CNS activity, or is something else going on?

---

## What I Did

I used RDKit to look at fluconazole through a computational lens and compare it to:
- other azoles (its natural “peer group”)
- known CNS-active drugs
- a bioactive natural compound (resveratrol)

Instead of focusing on one metric, I looked at multiple dimensions:
- polarity (TPSA)
- lipophilicity (LogP)
- flexibility (rotatable bonds)
- 3D character (FractionCSP3)

---

## What I Expected (and What I Didn’t)

I expected fluconazole might show *some* CNS-like characteristics.

It didn’t.

Across multiple views:
- It clusters with azoles, not CNS drugs
- It is more polar and less lipophilic than typical brain-penetrant compounds
- Its flexibility matches its class
- Its 3D character is slightly different—but not enough to explain CNS behavior

---

## What This Suggests

Fluconazole’s structure does **not** support efficient passive BBB penetration.

That creates a mismatch:

- Structure → not CNS-optimized  
- Observed biology → neuroprotective signal  

Which leads to a more interesting conclusion:

> The activity likely isn’t explained by passive diffusion alone.

More plausible explanations:
- transporter-mediated uptake  
- indirect pathway modulation  
- target-level effects not captured by simple descriptors  

---

## Why This Matters

This is a small example of a bigger idea:

> Structure-based rules are useful—but they don’t always tell the full story.

And when they don’t, that’s where the interesting science starts.

---

## Future Directions

- Molecular docking analysis to explore fluconazole's interaction with the IGF-1 receptor
  
- ADMET profiling to further characterize CNS penetration likelihood
  
- Comparative analysis with other repurposed neuroprotective compounds

## File

- `fluconazole_cadd_analysis.ipynb`


