## Financial Data Extraction 💵📑

Data extract from article that would expose as a table like structure. It can make easier to get the needed info from a given news article instead of read the whole article news.
The table contains the company name, stock symbol, revenue, net income, EPS. It specialized for commercial purpose.

Following picture is the interface >>>
![image](https://github.com/user-attachments/assets/d5e0044c-60b7-4bad-96b4-b4513473c6c3)

#### Prerequisites
- Python 3.9+
- openai API secret key
- openai package
- streamlit package

## Clone the repository
```
git clone https://github.com/fasinfasi/Financial-Data-Extraction.git
cd Financial-Data-Extraction
```

install packages
```
pip install openai
pip install streamlit
```

## Getting OpenAI API key
- create account in openai
- login with email
- Go to [https://platform.openai.com/apps](https://platform.openai.com/apps)
- Tap on API
- Give details
- Copy the api secret key (start with 'sk-')
#### Note:  OpenAI API key is sensitive information, and you must treat it as a secret to avoid unauthorized use. If someone else gets access to your API key, they could misuse it, leading to unexpected costs or violations of the OpenAI terms of service.

## To make the api secret key safe
### Step 1:
```
cd Financial-Data-Extraction
```
create a file name .env, then insert it
```
OPENAI_API_KEY = your_api_key
```
Then, Save it
### Step2:
Create .gitignore file and then just add
```
.env
```
Save it

Now the secret key is safe, No one to see when you make it public repo

## Use the .env File in Your Code
- In Python, install the python-dotenv library:
```
pip install python-dotenv
```
- Update your code to load the environment variable from the .env file:
```
from dotenv import load_dotenv
import os

# Load variables from .env
load_dotenv()

# Access the OpenAI API key
api_key = os.getenv("OPENAI_API_KEY")
```
Now the api key is ready!

## Usage
#### 1. Access the Streamlit's web app
- Open the frontend in your browser by run
``` streamlit run main.py ```
#### 2. Put the article
- Give the news article to the text area on the left side of the screen
- Tap on the Extract button
#### 3. View result
- The Extracted data will display on the right side table

Feel free to use and adapt this README! Let me know if you'd like further refinements🤗.
