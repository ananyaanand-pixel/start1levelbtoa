# Currency Converter CLI

A lightweight, terminal-based Python tool that allows users to quickly convert major global currencies into Indian Rupees (INR). It uses fixed exchange rates calibrated to August 24, 2026.

## ✨ Features

* Interactive CLI: Direct step-by-step terminal prompts for seamless operation.
* Case-Insensitive Parsing: Accepts uppercase or lowercase input letters seamlessly (E or e, W or w).
* Error Handling: Built-in catch for unrecognized currency symbols to prevent script crashes.
* Precise Math: Supports decimal input values for high-accuracy financial estimations.

------------------------------
## 💱 Supported Conversions
The script hardcodes specific currency evaluations based on late-August 2026 valuations:

| Base Currency | Expected Input | Code Implementation | Target Outcome |
|---|---|---|---|
| US Dollar ($) | $ | val * 95.68 | Converts to INR at ₹95.68 base |
| Euro (€) | e | val * 111.76 | Converts to INR at ₹111.76 base |
| British Pound (£) | p | val * 130.52 | Converts to INR at ₹130.52 base |
| South Korean Won (₩) | w | val * 0.069 | Converts to INR at ₹0.069 base |

------------------------------
## 🚀 Getting Started
## Prerequisites
You only need Python 3.x installed on your system. You can verify your installation by opening a command prompt/terminal and typing:

python --version

## Step-by-Step Execution

   1. Clone or Download: Save currency_converter.py to your machine.
   2. Open Terminal: Navigate to the folder directory where you saved the file:
   
   cd path/to/your/folder
   
   3. Run the Script: Launch the converter using Python:
   
   python currency_converter.py
   
   
------------------------------
## 💻 Code Breakdown
The application operates on an explicit conditional sequence:

   1. Introduction: Displays the supported parameters to the terminal user.
   2. Sanitized Input Collection: Normalizes input characters to lower-case values right away to match condition variables smoothly.
   3. Evaluation Matrix: Matches the sanitized symbol against explicit if/elif blocks to calculate the dynamic product output.

------------------------------
## 🛠 How to Modify Exchange Rates
Because exchange markets fluctuate daily, you can manually update the values by modifying the numeric multipliers inside the source code file. 

if sym=="$":
    print("value in inr is ", val * 98.50) # Change 95.68 to current market rate

------------------------------



