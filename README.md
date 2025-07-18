# **Package Sorter Project**

This project contains a simple Python function designed to sort packages into different stacks based on their dimensions and mass. It was developed focused for ease of use and testing.

## **How to Use**
Open the Google Colaboratory notebook and run all cells. 
[Link to open sorter_main_py.ipynb](https://colab.research.google.com/github/IkeSalmonson/sort_package/blob/main/sorter_main_py.ipynb)

## **Rules for Sorting**

The sort function classifies packages according to the following criteria:

A package is considered **bulky** if:

* Its volume (Width x Height x Length) is greater than or equal to 1,000,000 cm³.  
* OR, at least one of its dimensions (width, height, or length) is greater than or equal to 150 cm.

A package is considered **heavy** if:

* Its mass is greater than or equal to 20 kg.

Based on these rules, packages are classified to one of three stacks:

* **REJECTED**: Packages that are **both** heavy and bulky.  
* **SPECIAL**: Packages that are **either** heavy or bulky (but not both).  
* **STANDARD**: Packages that are **neither** heavy nor bulky.

## **Implementation**
### Sort Function
The core logic is contained in the sort(width, height, length, mass) function.
The notebook cell will create a sort.py containing the function definition to be used by the pytest.
### Testing 
The notebook cell will create a test_sort.py containing the test cases and function definition to be used by the pytest.
The last cell executes pytest as a command to run the testing suit. 
 

## **Testing**

The project uses the pytest library for testing. 
All covered test cases are declared as a list of expected inputs and outputs.

