# General Insurance Modelling - Domestic Car Insurance
### This repository showcases my modelling technique for a general insurance case.
The goal of this analysis is to figure out the best reinsurance for the company: 

 - no reinsurance,
 - an excess of loss on each claim, that would cover any excess over 1.5
   times the expected claim amount or,
 - an excess of loss on each policy aggregate (annual) cost, also
   covering any excess of 1.5 times the expectation (of aggregate policy
   claims paid over a year).

src\past_claims_data contains the claims data that is to be analysed. It consists of two columns: 

 - polind: policy number and
 - claim: size of the claim in dollars. If blank, this means that policy
   had no claim.

src\anaylsis_and_modelling.Rmd contains the source code for analysis, an R script is also available under the same name.

out folder contains all the output that is generated from the source codes.

Claims severity is generated from a gamma severity distribution with mean 874.4 and variance 76596.
Claims frequency is generated from a Poisson frequency with mean of 4.258.

© 2023 Edmund Liman All Rights Reserved