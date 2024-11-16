# **Ayat Text Extractor**  
A Python script to extract and clean Quranic verse texts from DOCX files. The script is designed to handle Word documents with metadata and list numbering, focusing only on extracting verse texts starting from the first ayah.

---

## **Features**
- Skips document metadata (e.g., surah names, Makkiyyah/Madaniyyah, and other headers).  
- Detects and processes list numbering automatically (e.g., "1.", "2)", etc.).  
- Cleans unnecessary numbering, footnotes, and spaces from verses.  
- Outputs normalized verse texts into a `.txt` file.  

---

## **Installation**  
Clone this repository:  
```bash
git clone https://github.com/username/ayat-text-extractor.git
cd ayat-text-extractor
```  

Install the required dependencies:  
```bash
pip install python-docx
```

---

## **Usage**
1. Place your DOCX files containing the Quranic text in a folder, e.g., `input_files`.  
2. Modify the `folder_path` and `output_folder` in the script:
   ```python
   folder_path = 'path_to_your_input_files'
   output_folder = 'path_to_your_output_folder'
   ```
3. Run the script:
   ```bash
   python extract_ayat.py
   ```
4. Extracted verses will be saved as `.txt` files in the output folder.

---

## **Example**  

### **Input DOCX:**
```
YŪNUS  
(YUNUS)  
Makkiyyah  
Surah ke-10 : 109 ayat  

Dengan nama Allah Yang Maha Pengasih lagi Maha Penyayang  
1. Alif Lām Rā. Itulah ayat-ayat Kitab (Al-Qur’an) yang penuh hikmah  
2. Pantaskah menjadi suatu keheranan bagi manusia bahwa Kami mewahyukan kepada seorang laki-laki di antara mereka...
```

### **Output TXT:**
```
Alif Lām Rā. Itulah ayat-ayat Kitab (Al-Qur’an) yang penuh hikmah  
Pantaskah menjadi suatu keheranan bagi manusia bahwa Kami mewahyukan kepada seorang laki-laki di antara mereka...
```

---

## **Folder Structure**
```bash
ayat-text-extractor/
├── input_files/             # Folder for input DOCX files
├── output_files/            # Folder for output TXT files
├── extract_ayat.py          # Main script
├── README.md                # Documentation
```

---

## **Contributing**
Feel free to fork this repository, create a branch, and submit a pull request if you'd like to contribute. Suggestions and issues are welcome in the [Issues tab](https://github.com/username/ayat-text-extractor/issues).

---

## **License**
This project is licensed under the MIT License. See `LICENSE` for details.

