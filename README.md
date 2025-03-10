# Text Mining (PubMed Search) with NLP & LLM 🚀

This project uses **NLP, LLM models, and text mining** to search **PubMed** for research articles related to specific **genes**. 
It integrates keyword expansion using **spaCy, NLTK, and MiniLM** for enhanced search accuracy.

This project leverages **NLP, LLM models, and text mining** to efficiently search **PubMed** for research articles related to specific genes. Even though Arabidopsis search is shown in the **colab notebook**. It can be extended to other organism as well. It integrates **keyword expansion** using **spaCy, NLTK, and MiniLM** to enhance search accuracy and improve literature retrieval.

## 🌟 Features  
✅ Retrieve PubMed articles using **gene symbols & TAIR IDs**  
✅ Expand search queries using **NLP models (spaCy, NLTK, MiniLM)**  
✅ Remove duplicate PubMed IDs & provide **clear logs**
✅ Fetch **detailed abstracts, DOI links, and matched keywords**

## Usage
**Prerequistes**
- **NCBI API Key**: Required for accessing PubMed efficiently
- **Hugging Face Token**: Needed for NLP model authentication (store in Colab secrets)

## Steps to Run
1️⃣ Enter **TAIR IDs or Gene Symbols** when prompted (*supports expansion to all organisms*)

2️⃣ Enter the **number of articles** to retrieve per search

3️⃣ The script will process **original and expanded queries** to retrieve PubMed articles


## 📊 Execution Flow
1. **User Input:** TAIR IDs / Gene Symbols
2. **Data Processing:** Extract TAIR IDs & Gene Symbols
3. **ID Conversion:** Convert TAIR IDs to Gene Symbols (if applicable)
4. **Keyword Expansion:** Use **NLP models** to generate related terms
5. **PubMed Querying:** Search using both **original & expanded keywords**
6. **Data Extraction:** Fetch article titles, abstracts, DOIs, and publication years
7. **Duplicate Removal:** Ensure **unique PubMed IDs** in results
8. **Final Output:** Display cleaned & structured search results

## 🛠️ Installation & Execution
1️⃣ **Clone the Repository**
   ```bash
   git clone https://github.com/sivkri/NLP-LLM-TextMining_GeneSearch.git
   cd NLP-LLM-TextMining_GeneSearch
   ```

2️⃣ **Run in Google Colab**

Simply upload and execute the provided Colab Notebook
```NLP-LLM-TextMining_GeneSearch.ipynb ```

##💡**Example Output**
 ```bash
Enter comma-separated TAIR IDs or gene symbols: AT4G26080, mapkkk18  
Enter the number of articles to retrieve per search (e.g., 5, 10, 15): 5  
✅ Results for AT4G26080: 0 (original) | 0 (expanded)  
✅ Results for mapkkk18: 5 (original) | 5 (expanded)  
✅ Results for ABI1: 5 (original) | 5 (expanded)  
⚠️ 10 duplicate PubMed ID(s) removed.  
```
