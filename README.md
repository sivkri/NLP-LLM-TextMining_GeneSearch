# PubMed Gene Search with NLP & LLM 🚀

This project uses **NLP, LLM models, and text mining** to search **PubMed** for research articles related to specific **genes**. 
It integrates keyword expansion using **spaCy, NLTK, and MiniLM** for enhanced search accuracy.

## 🌟 Features  
✅ Retrieve PubMed articles using **gene symbols & TAIR IDs**  
✅ Expand search queries using **NLP models (spaCy, NLTK, MiniLM)**  
✅ Remove duplicate PubMed IDs & provide clear logs  
✅ Fetch detailed abstracts, DOI links, and matched keywords  

## 🛠️ Installation  
1. Clone the repository:  
   ```bash
   git clone https://github.com/sivkri/NLP-LLM-TextMining_GeneSearch.git
   cd NLP-LLM-TextMining_GeneSearch

Usage
Enter TAIR IDs or Gene Symbols when prompted.
Enter the number of articles to retrieve per search.
The script will:
Retrieve gene symbols for TAIR IDs
Expand search queries using NLP models
Search PubMed using both original & expanded keywords
Remove duplicate PubMed IDs
Display results in a clickable table format

## 📊 Execution Flow
1️⃣ Extract TAIR IDs & Gene Symbols
2️⃣ Convert TAIR IDs to Gene Symbols (if needed)
3️⃣ Expand Search Keywords using NLP Models
4️⃣ Query PubMed using both original & expanded keywords
5️⃣ Fetch article details (Title, Abstract, DOI, Year)
6️⃣ Remove duplicate PubMed IDs & display results


## 💡 Example Output

Enter comma-separated TAIR IDs or gene symbols: AT4G26080, mapkkk18  
Enter the number of articles to retrieve per search (e.g., 5, 10, 15): 5  
 ```bash
✅ Results for AT4G26080: 0 (original) | 0 (expanded)  
✅ Results for mapkkk18: 5 (original) | 5 (expanded)  
✅ Results for ABI1: 5 (original) | 5 (expanded)  
⚠️ 10 duplicate PubMed ID(s) removed.  
