

## How it works

The application reads the PDF and splits the text into smaller chunks that can be then fed into a LLM. It uses OpenAI embeddings to create vector representations of the chunks. The application then finds the chunks that are semantically similar to the question that the user asked and feeds those chunks to the LLM to generate a response.

The application uses Streamlit to create the GUI and Langchain to deal with the LLM.


## Installation

To install the repository, please clone this repository and install the requirements:

```
pip install -r requirements.txt
```

You will also need to add your OpenAI API key to the `.env` file.

## Usage

To use the application, run the `main.py` file with the streamlit CLI (after having installed streamlit): 

```
streamlit run app1.py
```
.env example

 AICORE_AUTH_URL="https://*******.eu10.hana.ondemand.com/oauth/token"
 AICORE_CLIENT_ID='<clientID>'
 AICORE_CLIENT_SECRET='<clientsecret>'
 AICORE_BASE_URL="https://api.ai.prod.eu-central-1.aws.ml.hana.ondemand.com/v2"
 AICORE_RESOURCE_GROUP='<resource_group>'
