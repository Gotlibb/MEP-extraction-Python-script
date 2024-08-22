# MEP Extraction Script - Version 1.2

## Author: Gleb Perevoznyuk, HSE (2024)

This project contains a Python script for extracting and analyzing motor evoked potential (MEP) data from EEG recordings. The script automates the process of processing epochs and calculates the peak-to-peak amplitudes for various channels.

## Main Functions:

- **process_epochs_and_plot**: 
  Processes the epochs for each channel within each condition for each participant, calculates the peak-to-peak amplitude, and plots the results.

- **plot_epochs_for_all_channels**: 
  Plots all channels for each epoch, highlighting the peak and trough on each graph.

- **calculate_p2p_amplitude**: 
  Calculates the peak-to-peak amplitude for the provided epoch signal.

- **save_ptp_amplitude_to_excel**: 
  Saves the calculated peak-to-peak amplitudes to an Excel file for further analysis.

## Usage:

1. **Environment Setup:**
   - Ensure that all necessary Python libraries are installed. The project uses a specific environment named `mep_extr_env`, which can be created using Anaconda with the following command:
	conda create --name mep_extr_env
	conda activate mep_extr_env

   - After activating the environment, install the required packages using:
	pip install -r requirements.txt
   - If you have an `environment.yaml` file, you can create the environment directly from it:
	conda env create -f environment.yaml
	conda activate mep_extr_env
2. **Running the Script:**
- Open and run the `MEP_exctraction_V1.2.ipynb` file in Jupyter Notebook.
- Follow the instructions provided within the cells of the script.

3. **Saving Results:**
- After running the analysis, the results will be saved in an Excel file named according to the participant, in the specified folder.

## Notes:

- **Decimal Separators in Numeric Values:** 
The amplitude values are saved in the Excel file using commas as the decimal separator to ensure correct number recognition in Excel.

- **Compatibility:** 
The script has been tested on Python version 3.8 and higher. Make sure you are using a compatible Python version and have installed the necessary libraries to ensure the script runs correctly.

## Contact:

If you have any questions or issues, please contact the project author, Gleb Perevoznyuk - gotlibb@gmail.com.

