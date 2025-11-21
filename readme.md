# Ontario-Water-Level-Power-Revenue-Analysis

## Requirements
- You must have python and Jupyter installed to run the code.
- 

# Running the code
1. start by downloading the dependencies, by first creating a virtual environment
   ```bash
   python3 -m venv .venv
   ```
   Then activate the virtual environment:
   On macOS/Linux.
   ```
    source myenv/bin/activate
   ```
   On Windows (Command Prompt).
   ```bash
    .venv\Scripts\activate.bat
   ```

   Then download dependencies with the following command:
   ```bash
   pip install -r requirements.txt
   ```
3. Now that you have the requirements installed you can now run the code.

# Files
- 'Cornwall_data.csv' and 'Long_Sault_Dam_data.csv' are the original unfiltered datasheets.
- They contain mainly the water levels at each recorded time

- The 'clean/cornwall_final_data.csv' is the cleaned dataset, which merges the discharge (Q), with the waterlevel recorded at each time. Date, Time and Datetime are used for table merging purposes and make it easier to plot.

- The 'clean/cornwall_hourly_data.csv' is the same as 'cornwall_final_data.csv' except that we only have the rows on an hourly basis rather than showing the data at each recorded time.

- 'clean/Merged_hourly_data.csv' is the master dataset, with power, energy, date time, water level discharge per hour. It is missing revenue for now.
