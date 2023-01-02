# LanguageDAO-AI
Implementation of OpenAI GPT3 for the purpose of translating document from web3, as stewarded by LanguageDAO.

Great documentation here for using the API and fine-tuning:

https://beta.openai.com/docs/api-reference/introduction

https://beta.openai.com/docs/guides/fine-tuning

# Set API Key as Environmental Variable, for Mac Users 
Run this command in your terminal to open up your shell profile using the nano text editor.

nano ~/.zshrc

Add your OpenAI API Key in place of 'Your API Key'

export OPENAI_API_KEY= 'Your API Key'

By setting your API key as an environmental variable in your shell, 
you can reference it across terminal instances by using the os module
and calling 'os.getenv("OPENAI_API_KEY")'


# OpenAI suggests using their Command Line Interface
More here: https://beta.openai.com/docs/guides/fine-tuning

pip install --upgrade openai

openai tools fine_tunes.prepare_data -f <LOCAL_FILE>

openai api fine_tunes.follow -i <YOUR_FINE_TUNE_JOB_ID>
