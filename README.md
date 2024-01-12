SCRIPTS

Scripts should be run in numerical order, as they produce files used in the following scripts. Scripts 5.01 and 5.02 do not produce files used in the following scripts.

`02_exclude_participants.Rmd`: This documents the exclusion of participants due to health/developmental issues, language exposure criteria, and missing data in the English and French data sets separately.

`03_merge_english_and_french_to_estimate_word_and_concept_vocabulary_scores.Rmd` : This merges the English and French data sets and estimates vocabulary size for both languages combined as word and concept vocabularies.

`04_step_1_fit_logistic_curves.Rmd` : This excludes participants who were older than 18 months when they joined the study, then fits a logistic curve to individual data in each vocabulary type (single-language, word, and concept). A data frame with the midpoint, slope, and midpoint is created for further analyses.

`05_step_2_linear_and_mixed_effects_models.Rmd` : Main analyses script. Linear and mixed effects models are fit to vocabulary data with language exposure variables as predictors.

`05.1_identified_and_unidentified_vocabulary_spurt.Rmd` : Exploratory analyses script. Spurters' and non-spurters' vocabularies are compared at 18 and 30 months.

`05.2_reestimate_words_learned_during_spurt_Frank_etal_method.Rmd` : This documents the procedure used to estimate the number of words that participants learned during their vocabulary spurt.

`06_robustness_checks.Rmd` : This documents the robustness checks conducted. Results are reported in supplementary materials.

`07_manuscript.Rmd` : This script includes code that produces descriptions, figures, and tables used in the manuscript.


DATA

This folder includes all the csv files used and produced by the scripts. The number at the beginning of the file name corresponds to the number of the script that produced it (e.g., file "02_Eng_keepers" was produced by script "02_exclude_participants").
Some files do not have a corresponding script, as they were created manually or by scripts in other projects:

`01_Eng_columns.csv` : Anonymyzed English vocabulary data set.

`01_Fr_columns.csv` : Anonymyzed French vocabulary data set.

 `BabysNewWords_activity_status.csv` : Contains whether participants completed or withdrew from the study; it is used to exclude the latter.

 `ws_te_list_full.csv` : Contains a list of translation equivalents used to estimate concept vocbaulary size.
