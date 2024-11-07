# Chatbot "Sword" HR Assistant

## Description

The standard MS Azure AI Studio based solution, promoted as by default templetization by Microsoft.

* Front-end in *React.JS*
* Back-end in *Python*
* The corefunctionality is provided as API by Microsoft Azure.

## How to run it locally

Before cloning the repository, please make sure that you have:
* at least Python v. 3.11
* last Node.JS
well installed on your Win machine, then clone this repository.

Configure using your MS Azure AI Studio:
* ChatGPT models (v. >=3.5)
* Indexation Azure AI service (I have chosen text-ada02 , but you might use your configure) for your proper Q&A source file using which chatbot should answer on the custom questions
Test them inside Azure AI Studio before doing the next move.

Check & configure *.env* file, pay attention to the following params that you have to set:
* AZURE_OPENAI_RESOURCE= (note, not all URL but only the name, if not sure check python code where it called and complete URL formed)
* AZURE_OPENAI_MODEL=gpt-4 (my example)
* AZURE_OPENAI_KEY=<your_key_check_azure_ai_studio>
* AZURE_OPENAI_MODEL_NAME=gpt-4 (my example)
* AZURE_OPENAI_PREVIEW_API_VERSION=2024-05-13-preview (my example)
* AZURE_SEARCH_SERVICE=lx3ssbasic (my example, but it is related to how your configure indexing of your custom files for chatbot's Q&A)

Actually run *start.cmd*

## Disclaimer
More complicated usage that includes COSMOSDB approach is out of scope of this project.