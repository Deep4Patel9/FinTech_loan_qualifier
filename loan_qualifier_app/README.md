# Loan Qualifier App

This is a Python CLI(command-line interface) Application that allows the user to see the loan they qualify for from lenders without all the manual calculations and filtering. This application works by taking in a .csv file(an example is in the 'data' folder named 'daily_rate_sheet.csv') of loan criteria for various loan providers. You will be asked a number of questions through the command line to evaluate your eligibiliy for the given loans. Then an output will be provided for the number of loans that you are eligle for along with a prompt asking you if you want to save the information as a file, the path that you want to save to, and the name that you want to save the file as.


*Note: If you decide to create a more through .csv file of loan eligibily please enter this information into a .csv file the same way that it is listed below with a header:*

*Lender Name, Max Loan Amount, Max LTV (Loan-to-Value), Max DTI (Debt-to-Income), Min Credit Score, Interest Rate
*
---

## Technologies

This project uses python 3.7 with the following packages:

* [fire](https://github.com/google/python-fire) - For the command line interface, help page, and entrypoint.

* [questionary](https://github.com/tmbo/questionary) - For interactive user prompts and dialogs

---

## Installation Guide

Before running the application first install the following dependencies.

```python
  pip install fire
  pip install questionary
```

---

## Usage

To use the loan qualifier application simply clone the repository and run the **app.py** with:

```python
python app.py
```
*(Note: Make sure that you have navigated to the folder containing app.py in the terminal/gitbash and that you have all the dependencies installed along with python 3.7.)*

Upon launching the loan qualifier application you will be greeted with the following prompts.

The user just has to input the path of the file and then input the following infomation about the person looking for a loan :

Credit Score, Monthly Debt, Monthly Income, Desired Loan Amount, Home Value/Collateral

Then the application will go and filter through the list providing you with the amount of loans you qualify for based on the inputted .csv file. It will then ask if you would like to save the output as a .csv file, afterwards you will be prompted to enter the location that you would like to save the file to as well as the name of the .csv file. 

(Note: You will be prompted to enter all of this information in the command line.)

Congratulation now you have a file containing all the loans that you or your client are eligible.

---

## Contributors

Deep Patel --- deep4patel9@gmail.com

---

## License

MIT License