# SoS - Solution Simulator

<p align="center">
<img width="80" alt="icon" src="https://github.com/AnnaLivia/Case---Optimizing-Food-Donation-Delivery-for-Nonprofit-Company/assets/46559408/00659482-744b-476e-871e-8ef597b61d20")
</p>

**SoS** is an offline application for the case presented in

> A.L. Croella, M. Gregori, Case---Optimizing-Food-Donation-Delivery-for-Nonprofit-Company 
> to appear.
<br />

SoS is an offline application created using <a href="https://github.com/TomSchimansky/CustomTkinter">CustomTkinter, a python UI-library</a>.
Click <a href= "https://uniroma1it-my.sharepoint.com/personal/croella_1544694_studenti_uniroma1_it/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fcroella%5F1544694%5Fstudenti%5Funiroma1%5Fit%2FDocuments%2FDocumenti%2FEsercizi%5Fingegneria%2FLab%20RO%2FAltro%2FSAT%20material%2FSAT%20LogicaEco%20ITA%202023%2FCase%2D%2D%2DOptimizing%2DFood%2DDonation%2DDelivery%2Dfor%2DNonprofit%2DCompany&ga=1">here</a> to download it.
The repository constains two SoS application folders, <em>SoS\_win</em> and <em>SoS\_mac</em>, operating respectively under Windows and MacOS platforms.

<p align="center">
<img width="531" alt="Figure1" src="https://github.com/AnnaLivia/Case---Optimizing-Food-Donation-Delivery-for-Nonprofit-Company/assets/46559408/b9345b35-3287-4a49-99a3-5e317cba9765">
</p>

<p align="center"><b>Figure1:</b> SoS Home Frame.</p>


Each application consists in three nested folders: <em>\_data</em>, <em>\_input</em> and <em>\_output</em>.

#### Data
In the <em>\_data</em> folder, an Excel file named <em>Data.xlsx</em> stores all information needed in the assignment. In other words, it corresponds to the technical appendix that the Logica\&Co would have been supplying as attachment of its Call for Proposal. It includes:
<ul>
    <li> a list of all soup kitchen parameters (sheet <em>Soup Kitchens</em>);</li>
    <li> a list of all local businesses daily supply (sheet <em>Donations</em>);</li>
    <li> a list of all warehouses parameters (sheet <em>Warehouses</em>);</li>
    <li> a list of all sponsors parameters (sheet <em>Investments</em>);</li>
    <li> an origin-destination matrix of the distances from every warehouse to every local business (sheet <em>Distances W-LB</em>);</li>
    <li> an origin-destination matrix of the distances from every local business to every soup kitchen (sheet <em>Distances LB-S</em>);</li>
    <li> an origin-destination matrix of the distances from every soup kitchen to every warehouse (sheet <em>Distances S-W</em>);</li>
    <li> a list of supplementary parameters and coefficient (sheet <em>Additional Parameters</em>).</li>
</ul>

#### Input
The <em>\_input</em> folder contains solution-alike </em>.txt</em> files. It must be filled by the students (according to their selected approach) to run a simulation on the SoS and certify its goodness.

#### Output
The <em>\_output</em> folder is the target folder for simulation reports and contains the file <em>Technical\_sheet.txt</em> that summarizes all data reported in <em>Data.xlsx</em> and can be also printed through a SoS command. After a simulation is run, it is automatically populated with a variable summary file and a report (see the next section).

## How to use SoS
The SoS allows the students to investigate and check the framework data. Three command buttons in the <em>Home</em> frame enable the student to: 
<ul>
    <li> print the model parameters: a file named <em>Technical\_sheet.txt</em> is created in the <em>\_output</em> folder. It summarizes all model dimensions, parameters and constraints;</li>
    <li> upload, check and print the solution files provided by the students: the format of the files provided in the <em>\_input</em> folder is examined and, if no errors are detected, a summary file <em>Variables.txt</em> is created and saved in the  <em>\_output</em> folder. Otherwise, a popup window with an error report is displayed;</li>
    <li> perform a simulation using the uploaded values: the SoS checks if the proposed solution is feasible and publishes the results in the file <em>Report.txt</em> in the <em>\_output</em> folder. If the solution is acceptable, all revenues and costs are calculated in detail by day, month, and semester (total). In case of infeasible solution, a popup window with an error report is displayed; students can find specific details about the violated constraints in the report file.</li>
</ul>

Additionally, a <em>Map</em> frame provides a navigable map of all soup kitchens, local businesses and warehouses, and an <em>Info</em> frame presents the step-by-step procedure for running a simulation.
