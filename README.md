# Introduction
This is the supplementary material for an extensive production data set for a five-axis CNC milling process which can be found at Zenodo (https://doi.org/10.5281/zenodo.15735480). Three geometrically different products were manufactured and production data from the machine was recorded. The recorded manufacturing process contains the preparation of the machine for the next product (changeover) as well as the machining process (production). An experimental manufacturing was organized with the aid of a changeover matrix to ensure that all possible changeover combinations for the three products were considered. The production was repeated five times, resulting in 30 manufacturing sessions and five complete changeover matrices. The data set was recorded from a Siemens 840D-SL machine control on a five-axis milling machine tool of type "Spinner U5-620" in a laboratory environment. A rich feature set is provided including rich supplementary material i.e. the NC-codes of the products, tool information, and a Jupyter notebook to illustrate the usage of the dataset.

# Data descriptor
A data descriptor is available at Springer Scientific Data by Open access (https://doi.org/10.1038/s41597-025-05294-0).

# Content in the folders
The  following additional content can be found in the subfolders:
- Changeover process: Detailed description of the changeover process with flow chart
- NC code: NC-Code of the three example products
- Tool information: Detail information on the cutting tools used for milling
- Jupyter notebook: Example source code in Python, how to use the data set
- Data irregularities: List of interruptions
- Feature description: List of features and description
- Tool change: Additional information on how tools are changed on the "Spinner U5-620"

# Remark on file import and index in Python
Imoprting the csv with:
<pre> df = pd.read_csv(file_path,index_col=0) # Set the first column as the index </pre>
will result into an index with three vectors indicating the day changes between:
| Timestamp           | Index no. in csv | Vector no. |
|---------------------|------------------|------------|
| 12.03.2024 08:16:30 | 0                | 1          |
| ...                 | ...              | 1          |
| 12.03.2024 13:51:10 | 14331            | 1          |
| 20.03.2024 06:43:14 | 0                | 2          |
| ...                 | ...              | 2          |
| 20.03.2024 14:21:45 | 23831            | 2          |
| 22.03.2024 07:32:42 | 0                | 3          |
| ...                 | ...              | 3          |
| 22.03.2024 11:23:43 | 13861            | 3          |

You can return to a continuous index by dropping this index afterwards with:
<pre> df.reset_index(drop=True) </pre>

# Versions
- V1.0.0 Initial version (https://doi.org/10.5281/zenodo.14094886)
- V1.0.1 Fixed erratum (https://doi.org/10.5281/zenodo.15735480)
