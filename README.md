# Disk Image Forensics and File Recovery Toolkit

This repository provides a Python-based toolkit for disk image forensics and file recovery. It includes functionality to:
- Create disk images
- Verify data integrity using hash functions
- Recover deleted files (e.g., PDFs)
- Extract metadata from recovered images
- Generate comprehensive reports

This toolkit leverages libraries like `PyTSK3`, `PIL`, and `pandas` for efficient and automated recovery processes.

---

## **System Requirements**

### **Hardware**
- Minimum 4GB RAM (8GB recommended)
- 2 GHz dual-core processor
- At least 10GB free disk space

### **Operating System**
- Windows 10/11
- macOS 10.15 or later
- Linux (Ubuntu 20.04 or later recommended)

### **Software Dependencies**
- Python 3.8 or later
- Required Python libraries:
  - `os`
  - `hashlib`
  - `pytsk3`
  - `Pillow`
  - `pandas`

---

## **Installation Steps**

1. **Clone the Repository**
   ```bash
   git clone https://github.com/snehasonkusare-tech/Digital-Evidence-Recovery/blob/main/Digital%20evidence%20recovery.ipynb
   cd disk-image-toolkit
   ```

2. **Set Up a Python Virtual Environment (Optional)**
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/macOS
   venv\Scripts\activate   # Windows
   ```

3. **Install Required Python Libraries**
   ```bash
   pip install -r requirements.txt
   ```

4. **Verify Installation**
   Run the following command to check for missing dependencies:
   ```bash
   python -m pip list
   ```

---

## **Usage Instructions**

### **Step 1: Create a Disk Image**
Run the following command to create a disk image from a source file or drive:
```bash
python main.py --create-disk-image --source /path/to/source --output /path/to/output/disk_image.img
```

### **Step 2: Verify Data Integrity**
Calculate the hash of a file to verify its integrity:
```bash
python main.py --calculate-hash --file /path/to/file
```

### **Step 3: Recover Deleted Files**
Recover deleted files (e.g., PDFs) from a disk image:
```bash
python main.py --recover-files --disk-image /path/to/disk_image.img --output-dir /path/to/recovered_files
```

### **Step 4: Extract Metadata**
Extract metadata from recovered files:
```bash
python main.py --extract-metadata --file /path/to/recovered/file
```

### **Step 5: Generate Report**
Generate a detailed report of recovered files and metadata:
```bash
python main.py --generate-report --data /path/to/data.json --output /path/to/report.csv
```

---

## **Troubleshooting**

### Common Issues

1. **Missing Dependencies**
   - Ensure all required libraries are installed using:
     ```bash
     pip install -r requirements.txt
     ```

2. **Permission Errors**
   - Run the script with elevated privileges (e.g., `sudo` on Linux).

3. **File Not Found**
   - Double-check file paths for accuracy.

4. **PyTSK3 Not Installed**
   - Install PyTSK3 using:
     ```bash
     pip install pytsk3
     ```

5. **Unsupported File Format**
   - Ensure the files used are compatible with the toolkit (e.g., disk images, PDFs).

---

## **Support**
For any issues or feature requests, please open an issue on the [GitHub repository](https://github.com/snehasonkusare-tech/Digital-Evidence-Recovery).

