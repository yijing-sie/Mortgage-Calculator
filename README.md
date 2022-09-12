# Mortgage-Calculator
This is an assignment for Software Design for Visual Environments

* The goal is to build a simplified mortgage calculator that not only estimates the monthly mortgage payments but also **persists the data** for users to recover the results from their last use

* [mortgagev4](java/com/jblearning/mortgagev4) folder contains all my Java files 
* [res](res) folder contains the images and XML files for the UI of this application
* [Mortgage.java](java/com/jblearning/mortgagev4/Mortgage.java) implements the **shared preferences mechanism** to store and retrieve persistent data

* There are **3** mortgage parameters to use:  **mortgage amount** $M$, **annual interest rate** $R$, and **number of years** $Y$
  * **interest rate** is **compounded monthly**
* Monthly mortgage payment $P$ is computed according to the following equation:

$\huge P = {R\over 12} {M \over (1 - a ^{12Y})}$ where $\huge a = {1 \over 1+ {R\over12}}$

## Demo
Below is the demonstration of running Mortgage-Calculator on a real device (Samsung A71):


https://user-images.githubusercontent.com/84282744/189700641-3e783ad2-ebee-4b7b-aa9a-d37337bde8a1.mp4





* [report.pdf](report.pdf) demonstrates the correctness of the calculation in Mortgage-Calculator by comparing the results with those of an online mortgage calculator for twelve different cases 
