# PubMed Gene Search with NLP & LLM 🚀

This project uses **NLP, LLM models, and text mining** to search **PubMed** for research articles related to specific **genes**. 
It integrates keyword expansion using **spaCy, NLTK, and MiniLM** for enhanced search accuracy.

## 🌟 Features  
✅ Retrieve PubMed articles using **gene symbols & TAIR IDs**  
✅ Expand search queries using **NLP models (spaCy, NLTK, MiniLM)**  
✅ Remove duplicate PubMed IDs & provide clear logs  
✅ Fetch detailed abstracts, DOI links, and matched keywords  

## Usage
Prepare NCBI API Key by logging in.
Prepare the HuggingFace token id to save inn colab secrets.
Enter TAIR IDs or Gene Symbols when prompted. (It can be extended to all organisms)
Enter the number of articles to retrieve per search.


## 📊 Execution Flow
1. User inputs TAIR IDs / gene symbols
2. Extract TAIR IDs & Gene Symbols
3. Convert TAIR IDs to Gene Symbols (if needed)
4. Expand Search Keywords using NLP Models
5. Query PubMed using both original & expanded keywords
6. Fetch article details (Title, Abstract, DOI, Year)
7. Remove duplicate PubMed IDs & display results
8. Displays final results

## 🛠️ Installation  
1. Clone the repository:  
   ```bash
   git clone https://github.com/sivkri/NLP-LLM-TextMining_GeneSearch.git
   cd NLP-LLM-TextMining_GeneSearch
   
## 💡 Example Output
Enter comma-separated TAIR IDs or gene symbols: AT4G26080, mapkkk18  
Enter the number of articles to retrieve per search (e.g., 5, 10, 15): 5  
 ```bash
✅ Results for AT4G26080: 0 (original) | 0 (expanded)  
✅ Results for mapkkk18: 5 (original) | 5 (expanded)  
✅ Results for ABI1: 5 (original) | 5 (expanded)  
⚠️ 10 duplicate PubMed ID(s) removed.  
