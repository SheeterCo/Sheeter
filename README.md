# Sheeter 🖨️

Sheeter is your go-to project to easily convert Excel ⇄ JSON with handy cleaning scripts and well-organized logs.

## Versions history 📝

**[Latest (Beta 1)](https://github.com/TheLaval/Sheeter/releases/latest)**

- **[Beta 1](https://github.com/TheLaval/Sheeter/releases/tag/beta-1)**
- ...
- ...

## Important folder structure 🗂️

sheeter/
- input/ Edit files here (Excel & JSON)
- output/ Conversion results (Excel & JSON)
- clean/ Cleaning scripts for input/output (Excel & JSON)
- convert/ Conversion scripts Excel ⇄ JSON
- logs/ Logs of conversion processes (auto-generated)

---

# How to use Sheeter? 🤔

## Cleaners 🧹

There are 4 separate cleaning scripts to clean input or output files:

- Clean Excel input

- Clean Excel output

- Clean JSON input

- Clean JSON output

Each script deletes the targeted file if it exists.

## Input & Output folders 📥📤

Input: place your input.xlsx and input.json files here before converting.

Output: converted files like output.json and output.xlsx will be saved here.

⚠️ **Be careful not to rename the input/output file names! ALWAYS "input." or "output."**

## Logs 🗃️

All logs are saved inside the /logs folder

Log filenames follow this pattern:

[weekday]-[day]-[month]-[year]_[hour]h-[minute]m-[second]s_[index].log

Example: saturday-24-may-2025_20h-19m-05s_1.log

*Logs are written in English and include main steps and errors.*

*Logs are also printed in the console during script execution.*

---

# Notes 💬

Scripts automatically create necessary folders if they don’t exist.

Make sure your Excel and JSON files have the correct columns and format to avoid errors.

Close your Excel file if it’s open before running JSON → Excel conversion to prevent file lock issues.

Be careful not to rename the input/output file names! ALWAYS "input." or "output."

