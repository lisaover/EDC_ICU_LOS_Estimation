# EDC ICU LOS Estimation

This project was presented at the Annual Meeting of the American Medical Informatics Association in November 2023, New Orleans. The author list with complete affiliations are included at the end of the README.

## Repository files

* <code style="color : blue">Poster</code> P126_Over.pdf & P126_Over.png
* <code style="color : blue">Presentation Slides</code> P126_Over_slides.pdf
* <code style="color : blue">Abstract</code> Exploring an Imputation Strategy_Over
* <code style="color : blue">Calendar day calculation algorithm</code> get_calendar_days.ipynb & get_calendar_days.html
* <code style="color : blue">Algorithm processing example</code> Record_by_record_count.pdf

## Lin's Concordant Correlation Coefficient

Lin's Concordant Correlation Coefficient (CCC) was used to measure agreement between the ICU LOS reported in TQIP and two sets of values, separately, 1) the estimated ICU LOS from inhospital location data and 2) TQIP ventilation days. The CCC does not measure the linear relationship between variables and thus does not calculate a line of best fit. The CCC measures agreement between two judges or raters using the 45&deg; line or line of equality. The resulting CCC estimate indicates how well the data align with the line of equality. Lin's CCC is within a larger set of Intraclass Correlation Coefficients (ICC). Lin's CCC corresponds to the simplest ICC with two judges and one observation per patient.

The sample size for calculating the CCC was fixed because we drew a random sample of 1,115 (10%) from a fixed set of records (11,149) where ICU LOS and ventilation days are greater than zero, i.e., records assumed to be correct. The CCC between TQIP ICU days and the estimated ICU LOS from location records is 0.86 with 95% confidence interval (0.85, 0.88). We are 95% confident that the interval (0.85, 0.88) contains the true CCC between TQIP ICU days and estimated ICU days from location records. The CCC between TQIP ICU days and TQIP ventilation days is 0.72 with 95% confidence interval (0.69, 0.74). We are 95% confident that the interval (0.69, 0.74) contains the true CCC between TQIP ICU days and TQIP ventilation days. These two intervals do not overlap, therefore, we conclude that there is higher agreement between TQIP ICU days and the estimated ICU days from location records.

## Authors

Lisa Over, MLIS<sup>1,2</sup>, Kuo-Ting Huang, PhD<sup>2</sup>, Bryan A. Cotton, MD MPH<sup>3</sup>, Andrew Dennis, DO<sup>4</sup>, Francis Guyette, MD<sup>5</sup>, Brian Harbrecht, MD<sup>6</sup>, Bellal A. Joseph, MD<sup>7</sup>, Ernest Eugene Moore, MD<sup>8</sup>, Daniel G. Ostermayer, MD<sup>9</sup>, Silvia Owusu-Ansah, MD MPH<sup>10</sup>, Mayur B. Patel, MD MPH<sup>11</sup>, Martin Schreiber, MD<sup>12</sup>, Samual R. Todd, MD<sup>13</sup>, Chad T. Wilson, MD<sup>14</sup>, Stephen R. Wisniewski, PhD<sup>15</sup>, Jason Lee Sperry, MD MPH<sup>16</sup>

<sup>1</sup>University of Pittsburgh, Epidemiology Data Center; <sup>2</sup>University of Pittsburgh, Department of Information Culture and Data Stewardship; <sup>3</sup>University of Houston School of Medicine, Department of Surgery; <sup>4</sup>Cook County Health, Department of Trauma and Burn; <sup>5</sup>University of Pittsburgh School of Medicine, Department of Emergency Medicine; <sup>6</sup>University of Louisville School of Medicine, Department of Surgery; <sup>7</sup>University of Arizona Tucson College of Medicine, Department of Surgery; <sup>8</sup>University of Colorado Denver Health, Department of General Surgery; <sup>9</sup>University of Houston School of Medicine, Department of Emergency Medicine; <sup>10</sup>University of Pittsburgh School of Medicine, Assistant Professor of Pediatrics and Emergency Medicine; <sup>11</sup>Vanderbilt University Medical Center, Department of Surgery; <sup>12</sup>Oregon Health & Science University, Department of Surgery; <sup>13</sup>Grady Memorial Hospital, Department of Trauma Surgery; <sup>14</sup>Baylor College of Medicine, Department of Surgery; <sup>15</sup>University of Pittsburgh, School of Public Health; <sup>16</sup>University of Pittsburgh School of Medicine, Department of General/Trauma Surgery

