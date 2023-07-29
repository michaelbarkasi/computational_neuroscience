# computational_neuroscience
Templates and project code from 2023 Neuromatch Academy

neural_decoding_template_faux_data_simulation.ipynb

This CoLab first generates some faux sample fMRI data of somatomotor cortex during unilateral hand, unilateral foot, and tongue movements, then uses a GLM to decode the task from the data (logistic regression). The decoder was originally written to be used with the curated Human Connectome Project data released by Neuromatch Academy. It works pretty well with real data, but the HCP data has limitations on sharing, so for this demo I just use simulated data. The simulated data is at the region level (Brodmann regions, specifically).

GLM_of_task_dependent_correlation_faux_data_simulation_NMA_2023_Project.ipynb

This CoLab first generates some faux sample fMRI data of somatomotor cortex during unilateral hand, unilateral foot, and tongue movements, then uses a GLM to model one region's activity as a function of another region's activity, plus information about the laterality and extremity of the motor task being performed. It shows that the GLM does best when given all inputs, vs being given only another region's activity or only the extremity and laterality input.

GLM_template.ipynb

Sample code for doing GLMs, i.e. multi-dimensional linear regression. Specifically, it gives (a) an Linear-Gaussian Regression Model w/ L1 and L2 Regularization, and (b) an Linear-Poisson Regression Model w/ L2 Regularization. 
