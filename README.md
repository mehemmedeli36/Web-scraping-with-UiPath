# Web Scraping and Data Processing Automation with UiPath

An automated Robotic Process Automation (RPA) solution developed in UiPath that extracts specific data from web platforms, processes the collected information, and exports it into a structured Microsoft Excel report.

---

## 🚀 Project Overview

This project demonstrates a real-world business scenario where manual data extraction and reporting are transformed into a fully automated digital workflow. The automation is built using a **Modular Design Architecture** to ensure reusability, easy maintenance, and robust error handling.

### Key Features
* **Automated Web Navigation:** Dynamically opens the target browser, navigates to the specific web portal, and handles UI interactions.
* **Data Scraping:** Extracts structured or semi-structured data from web elements using optimized and dynamic UI selectors.
* **Data Manipulation & Architecture:** Utilizes `In/Out Arguments` to securely transfer data tables between isolated workflows.
* **Excel Automation:** Generates and formats Microsoft Excel reports dynamically based on the scraped dataset.
* **Exception Handling:** Embedded `Try-Catch` blocks to capture runtime errors and ensure process stability.

---

## 📁 Project Structure & Workflow Architecture

Instead of a monolithic design, the automation is broken down into functional components (workflows) invoked inside the `Main.xml`:

* **`Main.xaml`** - The central orchestrator of the automation logic.
* **`OpenBrowser.xaml`** - Handles browser initialization and navigation securely.
* **`DataScraping.xaml`** - Executes the data extraction wizard logic and captures data into a `DataTable`.
* **`WriteToExcel.xaml`** - Handles the file creation, structural formatting, and data writing processes.
* **`CloseApplications.xaml`** - Safely terminates browser sessions and Excel processes to ensure clean execution environments.

---

## 🛠️ Tech Stack & Prerequisites

* **RPA Platform:** UiPath Studio
* **Language Runtime:** C# / .NET
* **Dependencies:** * UiPath.System.Activities
    * UiPath.UIAutomation.Activities
    * UiPath.Excel.Activities

---

## ⚙️ Best Practices Applied

* **Clean Code & Naming Conventions:** Activities and workflows are clearly named to describe their functional intent.
* **Argument-Driven Data Flow:** Eliminated global variable dependencies by utilizing structured `In/Out` directional arguments.
* **Robustness:** Implemented fault tolerance mechanisms using Exception Handling structures to prevent abrupt robot failures.

---

## 🧑‍💻 Author

* **Əliyev Məhəmmədəli** - Aspiring RPA & Backend Developer
* GitHub: [@mehemmedeli36](https://github.com/mehemmedeli36)
