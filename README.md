# EDC ICU LOS Estimation

This project was presented at the Annual Meeting of the American Medical Informatics Association in November 2023, New Orleans. The author list with complete affiliations are included at the end of the README.

## Repository files

* <code style="color : blue">Poster</code> P126_Over.pdf & P126_Over.png
* <code style="color : blue">Presentation Slides</code> P126_Over_slides.pdf
* <code style="color : blue">Abstract</code> Exploring an Imputation Strategy_Over
* <code style="color : blue">Calendar day calculation algorithm</code> get_calendar_days.ipynb & get_calendar_days.html
* <code style="color : blue">Algorithm processing example</code> Record_by_record_count.pdf

## Questions and Answers

<strong>Why did you choose Lin's CCC over Pearson's correlation?</strong>
   
While both Lin's CCC and Pearson's correlation measure the strength of a relationship between two continuous variables, they serve different purposes. I chose Lin's CCC because I wanted to assess the agreement between two methods, accounting for both precision and accuracy. Pearson’s correlation, on the other hand, evaluates the linear association between two variables but does not necessarily imply agreement. In our context, it was more crucial to understand how closely our two methods agreed with each other, and that's why Lin's CCC was more appropriate.
 
<strong>Why didn't you use the Intraclass Correlation Coefficient (ICC)?</strong>
   
The Intraclass Correlation Coefficient (ICC) is an excellent tool for assessing the reliability or consistency of measurements or ratings within the same group. However, in our study, we were more focused on agreement between two different methods, rather than consistency or reliability within a single group. Lin's CCC provided a more direct measure of this concordance, making it a more suitable choice for our specific research question.

<strong>Why did you include the 85th percentile in Table 2: Summary of TQIP ventilation days by agreement with in-hospital ICU records?</strong>

The 85<sup>th</sup> percentile was included to show that the majority of values are 1 for the 518 records where TQIP and inhospital records agree that patients were not in the ICU. Of these 518 records, 52 were ventilated for two days (93<sup>rd</sup> percentile) and only nine records (98<sup>th</sup> percentile and above) had ventilation days greater than two. The low ventilation day values for these 518 records support the agreement between TQIP and inhospital location records and the decision not to impute the estimated ICU LOS for these records. The high ventilation day values for the 504 records where TQIP and inhospital records disagree support that patients were in the ICU and the decision to impute the estimated ICU LOS. 

## Authors

Lisa Over, MLIS<sup>1,2</sup>, Kuo-Ting Huang, PhD<sup>2</sup>, Bryan A. Cotton, MD MPH<sup>3</sup>, Andrew Dennis, DO<sup>4</sup>, Francis Guyette, MD<sup>5</sup>, Brian Harbrecht, MD<sup>6</sup>, Bellal A. Joseph, MD<sup>7</sup>, Ernest Eugene Moore, MD<sup>8</sup>, Daniel G. Ostermayer, MD<sup>9</sup>, Silvia Owusu-Ansah, MD MPH<sup>10</sup>, Mayur B. Patel, MD MPH<sup>11</sup>, Martin Schreiber, MD<sup>12</sup>, Samual R. Todd, MD<sup>13</sup>, Chad T. Wilson, MD<sup>14</sup>, Stephen R. Wisniewski, PhD<sup>15</sup>, Jason Lee Sperry, MD MPH<sup>16</sup>

<sup>1</sup>University of Pittsburgh, Epidemiology Data Center; <sup>2</sup>University of Pittsburgh, Department of Information Culture and Data Stewardship; <sup>3</sup>University of Houston School of Medicine, Department of Surgery; <sup>4</sup>Cook County Health, Department of Trauma and Burn; <sup>5</sup>University of Pittsburgh School of Medicine, Department of Emergency Medicine; <sup>6</sup>University of Louisville School of Medicine, Department of Surgery; <sup>7</sup>University of Arizona Tucson College of Medicine, Department of Surgery; <sup>8</sup>University of Colorado Denver Health, Department of General Surgery; <sup>9</sup>University of Houston School of Medicine, Department of Emergency Medicine; <sup>10</sup>University of Pittsburgh School of Medicine, Assistant Professor of Pediatrics and Emergency Medicine; <sup>11</sup>Vanderbilt University Medical Center, Department of Surgery; <sup>12</sup>Oregon Health & Science University, Department of Surgery; <sup>13</sup>Grady Memorial Hospital, Department of Trauma Surgery; <sup>14</sup>Baylor College of Medicine, Department of Surgery; <sup>15</sup>University of Pittsburgh, School of Public Health; <sup>16</sup>University of Pittsburgh School of Medicine, Department of General/Trauma Surgery

