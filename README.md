# seeq-f1
Framework to add F1 car telemetry into Seeq as signals

## Installation
To set up the project, follow these steps:

1. Clone the repository in to Seeq Data Lab:
Use the guide below for best practices
https://support.seeq.com/kb/latest/cloud/git-integration-with-seeq-data-lab

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```
## Usage
Navigate to the Create_Telemetry_Signals.ipynb notebook

Review the default contant values 
**WORKBOOK_NAME** is important as this will keep all of your signals scoped to just the designated workbook 
This will mean that telemetry signals will not be discorable in other workbooks

**DATASOURCE_NAME** will create a new datasource and the system and will make is simple to find and modify signals in the future

Run the all cells in the notebook. It will create a flat list of signals and conditions in the following format **season.team.carnumber.sensor_name**

For data analysis and visualization, open seeq workbench to the scoped notebook, search for the signals and have fun


## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.
