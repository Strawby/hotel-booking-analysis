# Hotel Booking Analysis

This repo contains a Jupyter notebook for exploring hotel booking data.

## Project Structure

```text
data/
  raw/bookings.csv
  processed/clean_bookings.csv
notebooks/
  hotel_analysis.ipynb
reports/
```

## Install Python

This notebook uses Python 3. If `python --version` does not work on Windows, install Python from:

https://www.python.org/downloads/

During installation, check **Add python.exe to PATH**.

After installing, open a new PowerShell window and confirm:

```powershell
python --version
```

## Create And Activate A Virtual Environment

From the repo root:

```powershell
cd C:\Users\India\Documents\Projects-Dani\hotel-booking-analysis
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

If PowerShell blocks activation, run this once in the same PowerShell window:

```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
.\.venv\Scripts\Activate.ps1
```

## Install Dependencies

With the virtual environment active:

```powershell
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
python -m ipykernel install --user --name hotel-booking-analysis --display-name "Python (hotel-booking-analysis)"
```

## Run The Notebook

The notebook reads data using paths relative to the `notebooks` folder, so start Jupyter from there:

```powershell
cd notebooks
jupyter notebook hotel_analysis.ipynb
```

In the browser, choose the kernel named:

```text
Python (hotel-booking-analysis)
```

Then run the cells from top to bottom.

## Data Files

The notebook expects this input file:

```text
data/raw/bookings.csv
```

It writes the cleaned output here:

```text
data/processed/clean_bookings.csv
```
