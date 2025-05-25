# ☕ Sheeter — JSON ⇄ Excel Converter

**Sheeter** is your Python tool to convert between **Excel and JSON** files, with **smart file handling**, **clean logging**, and **auto-detection** of formats. From input cleaning to cross-platform compatibility and Excel lock prevention — Sheeter makes the job smooth and safe.  

---

## 🔁 Beta 1 vs Beta 2 Comparison

| Feature / Change                                  | Beta 1                          | Beta 2 ✅                        |
|---------------------------------------------------|----------------------------------|----------------------------------|
|  File lock detection (`is_file_locked`)         | ❌ Not implemented               | ✅ Checks if input/output files are locked |
|  Prompt to auto-close Excel if opened           | ❌ No prompt                     | ✅ Cross-platform auto-close prompt |
|  Logs with timestamped filenames                | ⚠️ Simple log                    | ✅ Unique timestamped logs per run |
|  Output file resizing (Excel)                   | ❌ No formatting                 | ✅ Auto-adjust column width      |
|  Input validation for Excel (key/value)         | ❌ Might crash                   | ✅ Checks for `key` and `value` columns |
|  Error handling                                 | ⚠️ Minimal try/except            | ✅ Structured error messages with logging |
|  Folder structure (`input`, `output`, `logs`)   | ⚠️ Manual                        | ✅ Auto-created at runtime       |
|  Conversion supported                           | ⚠️ JSON → Excel only               | ✅ Both directions supported     |
|  User interaction                               | ❌ None                         | ✅ Yes/No input for closing Excel |
|  Check if Excel is open in browser              | ❌ Not considered                | ✅ Works even if opened via browser |
|  Format detection (dict/list) in JSON           | ❌ Static                        | ✅ Auto-converts dict to list    |

✅ **Beta 2 = More safe, more clean, more smart.**

---

## 📦 Project Structure

sheeter/

├── input/ # Drop your Excel (.xlsx) or JSON (.json) files here

├── output/ # Converted files (output.xlsx or output.json)

├── convert/ # Conversion scripts: JSON ⇄ Excel

├── clean/ # Optional cleaners for input/output files

├── logs/ # Logs auto-generated for each conversion


---

## 🚀 How to Use Sheeter

### 🔁 Converters

- **JSON → Excel**: Reads JSON (list or dict) and writes Excel file
- **Excel → JSON**: Reads Excel with 'key' and 'value' columns and writes JSON

Each script:
- Validates file formats
- Checks if files are open or locked
- Logs all steps and errors
- Adjusts Excel column width for readability

### 🧹 Cleaners

There are 4 separate cleaning scripts to clean input or output files:
- Clean Excel input
- Clean Excel output
- Clean JSON input
- Clean JSON output

Each script deletes the corresponding file if it exists.

---

## 📥 Input & Output

- **input/** → `input.json` / `input.xlsx`
- **output/** → `output.json` / `output.xlsx`

⚠️ **Do not rename input/output filenames — they must stay "input." or "output."**

---

## 📄 Logs

- All logs go into `/logs/` folder
- File format:

saturday-24-may-2025_20h-19m-05s_1.log

- Logs include steps, warnings, and errors (in English)
- Printed both to file and console

---

## 🔐 Tips

- Always close your Excel file before converting to avoid lock issues
- JSON must be a list of objects or a dictionary
- Excel file must contain columns: `key`, `value`
- Wanna see version history? [Go here](https://github.com/SheeterCo/Sheeter/blob/main/HISTORY.md)

---

Sheeter — The cheat code for your sheets. 🧑‍💻

Made with 💻 by [SheeterCo.](https://github.com/SheeterCo/) ([TheLaval](https://github.com/TheLaval))
