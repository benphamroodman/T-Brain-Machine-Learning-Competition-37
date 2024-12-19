# T-Brain Machine Learning Competition 37: RAG for Financial Data

---

Final submission to T-Brain's 37th competition: Creating an RAG from sample data to answer ambiguous questions about finance, insurance, or other, with IDs of the relevant documents.

We achieved the best results with minimal data pre-processing. Our RAG method relies on the Beijing Academy of Artifical Intelligence's (BAAI) reranker model to sort documents by relevance to the query. Then it chunks the top three and reranks them again, returning the top result.

Best accuracy on sample data: 136/150 (90.7%).

To test, run fintech.ipynb (Requires JupyterLab or Jupyter Notebook). Required Python packages: json, tqdm, torch, transformers, os.

