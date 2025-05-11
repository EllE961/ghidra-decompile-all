# 🔍 Ghidra Bulk Decompiler Export Script

This script exports **all decompiled functions** from a binary loaded in [Ghidra](https://ghidra-sre.org/) into a single `.txt` file using the Ghidra Decompiler API.

Created by **EllE**, this tool is helpful for reverse engineers and CTF players who want to analyze or share all decompiled code at once.

---

## 📜 Features

- Decompile **all functions** in the current program.
- Output clean, readable **C code** for each function.
- Save to a single output `.txt` file.
- Automatically handles errors and logs failed decompilations.

---

## 🚀 Usage

### 1. Load the Script in Ghidra

1. Open your Ghidra project and load a binary.
2. Open **Script Manager**: `Window → Script Manager`.
3. Click **"New Script"**, choose Python.
4. Paste in the code from `ExportAllDecompiledFunctions.py`.
5. Save the script.

### 2. Run the Script

1. Select the script from the Script Manager.
2. Click **Run**.
3. Choose an output directory when prompted.
4. A text file like `yourbinary_decompiled.txt` will be saved in that directory.

---

## 📂 Output Example

```c
/* Function: main */
void main() {
  ...
}

/* Function: validate_input */
bool validate_input(char *input) {
  ...
}
````

---

## 📎 Requirements

* Ghidra 10.x or newer
* Ghidra Python (Jython) scripting enabled

---

## 📖 License

MIT License — free to use, modify, and share.

---

## ✍️ Author

**EllE**
A reverse engineer and developer who builds tools for speed, clarity, and precision.
