# Stress-Predict Dataset

Ensure that the folder containing the dataset is inside the same path as the Jupiter notebook.
The Jupiter notebook lists all dependencies in the start, ensure these are installed within the environment before running the notebook.
use either pip or Conda to install before running if any are missing.

The notebook contains clear sections to demonstrate what is happening, all paths are written to be independent of the global path if the notebook is in the same folder as the folder containing the data.
All code is self-contained within the notebook and does not have any external dependencies other than libraries to be installed in the environment.


## Dataset Files

#### |-- Processed_data 

            |-----Improved_All_Combined_hr_rsp_binary.csv (contain information of heart rates and respiratory rates of all the participants along with timestamps and labels (for nonstress/baseline and 1 for stress task duration))

            |-----Questionnaires_scores.xlsx (contains information about the PSS and STAI questionnaire scores of each participant)

            |-----Time_logs.xlsx (contain date and start/end time of each task for each participant, Irish standard time)

#### |-- Raw_data

            |-----SX Folder (folders with raw files from Empatica E4. Where X is participant number)

                  |-----ACC.csv (contains accelerometer data (x, y, z axis))

                  |-----BVP.csv (contains raw BVP data)

                  |-----EDA.csv (contains EDA data (skin conductance))

                  |-----HR.csv (contains heart rate data)

                  |-----IBI.csv (contains inter-beat-interval data)

                  |-----info.txt (contains information about all the csv file and sampling rate)
     
                  |-----tags_SX.csv (contains timestamp tags. start-end time of each task)

                  |-----TEMP.csv (contains skin temperature data)

These all files in dataset files are used from original dataset.

## Libraries

Following libraries were used for analysis:

- Statistical Analysis (Rstudio):
  - Numpy
  - Pandas
  - Matplotlib
  
- Descriptive Analysis (python):
  - Pandas
  - Numpy
  - matplotlib
- Classification Analysis (python):
  - Numpy
  - Scikit-learn
  - Decision Tree
  - Gradient Boost Classifier
  - Scipy
  - Pickle
  

## References

**When using this dataset, please cite the following:**

1.	N. C. Basjaruddin, F. Syahbarudin, and E. Sutjiredjeki. Measurement device for stress level and vital sign based on sensor fusion. Healthcare Informatics Research, 27(1):11–18, 2021.
2. Talha Iqbal, Adnan Elahi, Sandra Ganly, William Wijns, and Atif Shahzad. _"Photoplethysmography-Based Respiratory Rate Estimation Algorithm for Health Monitoring Applications."_ Journal of medical and biological engineering 42, no. 2 (2022): 242-252. https://doi.org/10.1007/s40846-022-00700-z
3.	T. Iqbal, A. J. Simpkin, D. Roshan, N. Glynn, J. Killilea, J. Walsh, G. Molloy, S. Ganly, H. Ryman, E. Coen, et al. Stress monitoring using wearable sensors: A pilot study and stresspredict dataset. Sensors, 22(21):8135, 2022. 
4.	B. Szakonyi, I. Vass´anyi, E. Schumacher, and I. K´osa. Efficient methods for acute stress detection using heart rate variability data from ambient assisted living sensors. BioMedical Engineering OnLine, 20(1):1–19, 2021.