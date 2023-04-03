# Introduction

- Overview of the purpose of this book
- Guide for the end users of AMISR data
- General ISR theory
- Applied technique and radar operations
- Accessing data - guide of SRI database
- Using data appropriately
- AC vs LP
- error handling
- Examples of more sophisticated plots/analysis

## Incoherent Scatter Radar

Incoherent Scatter Radars (ISRs) are large, ground-based facilities that measure ionospheric plasma parameters in the upper atmosphere.  They have been used for decades to investigate ionospheric plasma dynamics and are particularly powerful for their ability to measure a profile of plasma parameters through the entire ionospheric layer.  The four basic plasma parameters ISRs can measure are:

- Electron Density (Ne)
- Ion Temperature (Ti)
- Electron Temperature (Te)
- Line-of-Site Plasma Velocity (Vlos)


## AMISR Basics

Advanced Modular Incoherent Scatter Radars (AMISR) are a special category of ISR that are electronically-steerable phased-array radars. This means that the beam direction is set by individually varying the phase of each transmitting element such that constructive interferance occurs in the desired direction.  Because these phase shifts are enforced electronically and there is no need to physically move the radar structure, the beam look direction can be altered multiple times per second.  This allows the radar to cycle through a set of a set of independent look directions many times in one integration period, effectively measuring a volume of ionospheric plasma (instead of just one profile) simultaniously.

![pfisr_array](images/pfisr_array.png)