# SoS - Solution Simulator

<p align="center">
<img width="80" alt="icon" src="https://github.com/AnnaLivia/Case---Optimizing-Food-Donation-Delivery-for-Nonprofit-Company/assets/46559408/00659482-744b-476e-871e-8ef597b61d20")
</p>

**SoS** is an offline application for the case presented in

> A.L. Croella, M. Gregori, Case---Optimizing-Food-Donation-Delivery-for-Nonprofit-Company to appear

<br>

SoS is an offline application created using [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter), a Python UI library. 
Click [here](https://uniroma1it-my.sharepoint.com/:f:/g/personal/croella_1544694_studenti_uniroma1_it/Elyvsz3bjClBoFEhHI0Ff5kB2QqCcwYiOCmAqz0vxt8FvA?e=gxSzC6) to download it.
<br>
The application is compatible with Windows and macOS platforms.

> [!IMPORTANT]
> On macOS put the app in quarantine platforms by running the following command in a terminal:<br>
> <em>xattr -d com.apple.quarantine your/path/to/SoS/SoS_mac.app</em>

<br>
<br>

<p align="center">
<img width="531" alt="Figure1" src="https://github.com/AnnaLivia/Case---Optimizing-Food-Donation-Delivery-for-Nonprofit-Company/assets/46559408/b9345b35-3287-4a49-99a3-5e317cba9765">
</p>

<p align="center"><b>Figure1:</b> SoS Home Frame.</p>

SoS needs three folders to be run: <em>data</em>, <em>input</em> and <em>output</em>.

#### Data
The <em>data</em> folder contains an Excel file named <em>Data.xlsx</em> with all the data required to model the Logica&Co problem. It includes:
<ul>
    <li> a list of all soup kitchens' parameters (sheet <em>Soup Kitchens</em>);</li>
    <li> a list of all local businesses' daily supply (sheet <em>Donations</em>);</li>
    <li> a list of all warehouses' parameters (sheet <em>Warehouses</em>);</li>
    <li> a list of all sponsors' parameters (sheet <em>Investments</em>);</li>
    <li> an origin-destination matrix of the distances from every warehouse to every local business (sheet <em>Distances W-LB</em>);</li>
    <li> an origin-destination matrix of the distances from every local business to every soup kitchen (sheet <em>Distances LB-S</em>);</li>
    <li> an origin-destination matrix of the distances from every soup kitchen to every warehouse (sheet <em>Distances S-W</em>);</li>
    <li> a list of supplementary parameters and coefficients (sheet <em>Additional Parameters</em>).</li>
</ul>
<p>
A file named <em>Data.txt</em>, summarizing all data reported in <em>Data.xlsx</em> in a text file, can also be generated using a SoS command <code>Print</code>.
</p>

#### Input
The <em>input</em> folder contains solution-alike </em>.txt</em> files.  To evaluate the quality of a proposed solution, this folder must be populated with the solution data by the users.

#### Output
The <em>output</em> folder is the target folder for the simulation reports. After a simulation, the <em>\output</em> folder is automatically populated with a variable summary file and a report.

## How to use SoS
<p>
The SoS allows users to gain insights into a solution and inspect the framework data. A Map frame provides a navigable map of all soup kitchens, local businesses, and warehouses, and an Info frame summarizes the step-by-step procedure for running a simulation.
</p>
<p>
Within the Home frame, there are three command buttons:
</p>
<ul>
<li> <code>Print</code>: Print the model parameters in a file named <em>Data.txt</em> in the data folder. This file summarizes all model dimensions and parameters.
</li>
<li> <code>Upload</code>: Upload, check, and print the solution files inserted by the user in the input folder. If no errors are detected, a summary file <em>Variables.txt</em> is created and saved in the output folder; otherwise, a popup window with an error report appears.
</li>
<li> <code>Run simulation</code>: Run a simulation using the uploaded input values. If the inputs produce a feasible solution, all revenues and costs are calculated in detail by day, month, and semester (total) and stored in a file named <em>Report.txt</em> in the output folder. If the inputs lead to an infeasible solution, a popup window with an error report appears; details on the violated constraints can be found in the <em>Report.txt</em> file.
</li>
</ul>
