<p align="center">
 <img width="100px" src="https://github.com/user-attachments/assets/0b6e0abf-970e-4cea-b504-c812b8d8bd5d" align="center" alt="GitHub Readme Stats" />
 <h2 align="center">Sheeter (SheeterCo.)</h2>
 <p align="center">Python tool to convert between Excel and JSON files!</p>
</p>

<p align="center">
  <!-- Latest release -->
  <a href="https://tooomm.github.io/github-release-stats/?username=SheeterCo&repository=Sheeter">
    <img alt="Latest Release" src="https://img.shields.io/github/v/release/thelaval/Sheeter?style=flat&logo=python&logoColor=black&label=Latest%20Release%20%3A&labelColor=white&color=green" />
  <!-- Downloads -->
  <a href="https://tooomm.github.io/github-release-stats/?username=SheeterCo&repository=Sheeter">
    <img alt="Downloads" src="https://img.shields.io/github/downloads/thelaval/Sheeter/total?style=flat&logo=github&logoColor=black&label=Downloads%20%3A&labelColor=white&color=turquoise" />

  <!-- GitHub stars -->
  <a href="https://github.com/SheeterCo/Sheeter/stargazers">
    <img alt="GitHub stars" src="https://img.shields.io/github/stars/thelaval/Sheeter?style=flat&logo=github&logoColor=black&label=Stars%20%3A&labelColor=white&color=gold" />
  </a>
</p>

# 📦 Project Structure

sheeter/

├── input/ # Drop your Excel (.xlsx) or JSON (.json) files here

├── output/ # Converted files (output.xlsx or output.json)

├── convert/ # Conversion scripts: JSON ⇄ Excel

├── clean/ # Optional cleaners for input/output files

├── logs/ # Logs auto-generated for each conversion

# 🚀 How to Use Sheeter

## 🔁 Converters

- **JSON → Excel**: Reads JSON (list or dict) and writes Excel file
- **Excel → JSON**: Reads Excel with 'key' and 'value' columns and writes JSON

Each script:
- Validates file formats
- Checks if files are open or locked
- Logs all steps and errors
- Adjusts Excel column width for readability

## 🧹 Cleaners

There are 4 separate cleaning scripts to clean input or output files:
- Clean Excel input
- Clean Excel output
- Clean JSON input
- Clean JSON output

Each script deletes the corresponding file if it exists.

## 📥 Input & Output

- **input/** → `input.json` / `input.xlsx`
- **output/** → `output.json` / `output.xlsx`

⚠️ **Do not rename input/output filenames — they must stay "input." or "output."**

## 📄 Logs

- All logs go into `/logs/` folder
- File format:

saturday-24-may-2025_20h-19m-05s_1.log

- Logs include steps, warnings, and errors (in English)
- Printed both to file and console

# 🔐 Tips

- Always close your Excel file before converting to avoid lock issues
- JSON must be a list of objects or a dictionary
- Excel file must contain columns: `key`, `value`
- Wanna see version history? [Go here](https://github.com/SheeterCo/Sheeter/blob/main/HISTORY.md)

---

Sheeter — The cheat code for your sheets. 🧑‍💻

Made with 💻 by [SheeterCo.](https://github.com/SheeterCo/) ([TheLaval](https://github.com/TheLaval))
