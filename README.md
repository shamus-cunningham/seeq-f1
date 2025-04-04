# seeq-f1
A framework for integrating F1 car telemetry data into Seeq as signals.

## Installation

To set up the project in **Seeq Data Lab**, follow these steps:

1. **Clone the repository**  
   Use Seeq's Git integration best practices as outlined here:  
   [Git Integration with Seeq Data Lab](https://support.seeq.com/kb/latest/cloud/git-integration-with-seeq-data-lab)

2. **Install required dependencies**  
   Run the following command in your environment:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Open the `Create_Telemetry_Signals.ipynb` notebook.

2. Review and set the following constants:
   - `WORKBOOK_NAME`: This value scopes all telemetry signals to a specific workbook, ensuring they are not discoverable in other workbooks.
   - `DATASOURCE_NAME`: This creates a new data source in Seeq, making it easier to locate and manage your signals.

3. Run all cells in the notebook.  
   This will generate a flat list of signals and conditions using the format:  
   ```
   season.team.carnumber.sensor_name
   ```

4. Once the signals and conditions are created, open the `F1_Car_Asset_Structure.ipynb` notebook.  
   This notebook builds the asset tree to organize your signals and conditions. You can also define templated calculations here to include any formulas or metrics within the asset structure.

5. For analysis and visualization, open Seeq Workbench to the specified workbook, search for your signals, and start exploring the data!

## Contributing

Contributions are welcome!  
Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License.  
See the [LICENSE](./LICENSE) file for more information.
