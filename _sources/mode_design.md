# Basics of Mode Design

## Pulse Coding
AKA: LP vs AC

TDLR; For F-region experiments, use long pulse data
For E-region experiments, use alternating code data

## Beam Positions
AMISRs are electronically-steerable phased-array radars, meaning the beam direction is set by individually varying the phase of each transmitting element such that constructive interferance occurs in the desired direction.  Because these phase shifts are enforced electronically and there is no need to physically move the radar structure, the beam look direction can be altered multiple times per second.  This allows the radar to cycle through a set of a set of independent look directions many times in one integration period, effectively measuring a volume of ionospheric plasma (instead of just one profile) simultaniously.

## Range Resolution
Post processing

## Integration Period
The integration period is the length of time autocorrelation functions are summed over before fitting to the ISR spectrum to determine plasma parameters.  This is determined in post-processing, and often raw data from one experiment is processed with mulitple integration periods.  The longer the integration period, the more independent pulses contribute to the spectrum, which because the ISR technique is inherently statistical, results in higher confidence in the fitted parameters.  In short, a longer integration period will ususally mean less noisy data with few errors. However, long integration periods will also have lower temporal resolution and may smear out sharp transient features.  In general, you should chose the longest integration period that still captures the time scales of interest for the phenomena you are studying.

## Common Operation Modes