<p  align="center">

<img  src="resources/logo_2.png"  height=300  width=300/>

</p>

# <p style="font-family:Droid Serif"><center>A suite of NLP tools to simplify legal documents</center></p>
  
  
### What do employment agreements, contracts, lease documents, patents and licenses have in common?
Apart from the fact that they're all legal documents:
1. They tend to have complex sentence structure and vocabulary choices that aren't accessible to people only familiar with conversational English
2. Are difficult to comprehend for non-native speakers of the language they are written in
3. Can run into several tens of pages (if not more)
  
  
## <font face="Trebuchet MS" color='maroon'>Legal-chat</font> addresses these issues using three tools:

1.  **QnA over legal documents**: Copy your document and ask it questions. Useful whether you have questions about the document as a whole or a specific clause.

2.  **Document summarization**: Generate a summary of the document. Options include changing the length of the summary (`small`, `medium` or `large`) and a choice between `paragraphs` or `bullets`. 

3.  **Multi & Cross-lingual document search**: Perform cross-lingual semantic search over a collection of legal documents. This is currently a showcase feature allowing the user to perform keyword as well as semantic search over a collection of COVID-19 pandemic legislative documents and returns the top-3 document matches. Also features the option to translate into other languages [currently English-only].
  
  
## **Installation:**

1. Create a free-tier Cohere account and set the COHERE_API_KEY environment variable.

2. Create a free-tier Qdrant cluster and set the following environment variables - QDRANT_API_KEY AND QDRANT_HOST.

3. Install requirements.

```
cd <project_dir>

conda create -n legal-chat --file requirements.txt

conda activate legal-chat
```
  
  
## **Usage**
In the project dir, run:
```
python gradio_demo.py
```

To run the app in reload mode:
```
gradio gradio_demo.py
```
 
The app should typically appear on the url: `http://localhost:7860`

<p  align="center">

<img  src="resources/sample.png" />

</p>
  
  

## Tools & Technologies used:

1. **[Cohere](https://docs.cohere.ai/docs/the-cohere-platform)**

2.  **[Qdrant](https://qdrant.tech/)**

3.  **[Langchain](https://langchain.readthedocs.io/en/latest/getting_started/getting_started.html)**

4.  **[Gradio](https://gradio.app/docs/)**