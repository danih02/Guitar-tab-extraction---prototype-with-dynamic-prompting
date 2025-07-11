# Guitar-tab-extraction---prototype-with-dynamic-prompting

# Guitar Tab Extraction - Prototype with Dynamic Prompting

This project is a prototype for extracting guitar tabs from PDF documents using multimodal large language models (LLMs) and computer vision techniques. The workflow demonstrates dynamic prompting, iterative feedback, and integration with Google Gemini and Ultralytics for image analysis.

## Features

- **PDF to Image Conversion:** Extracts images from PDF files for tab analysis.
- **Gemini 2.5 Flash Integration:** Uses Google's multimodal LLM to interpret tab images and output guitar tablature.
- **Dynamic Prompting:** Implements a feedback loop where the LLM learns from its mistakes through user corrections.
- **Tab Formatting:** Outputs extracted tabs in a readable, horizontal format.
- **Object Detection:** Utilizes Ultralytics and Gemini for detecting measures and numbers in tab images.
- **Visualization:** Annotates and displays detected objects on tab images.

## Usage

1. **Install Dependencies**
   - Run the following in a notebook cell:
     ```python
     %pip install langchain_google_genai google-genai ultralytics
     ```

2. **Set Up API Keys**
   - Set your `GOOGLE_API_KEY` as an environment variable.

3. **Run the Notebook**
   - Open `Guitar tabs extraction - prototyping.ipynb` and execute cells sequentially.

4. **Dynamic Feedback**
   - Follow the prompts to approve or correct the LLM's output for each measure.

## File Structure

- `Guitar tabs extraction - prototyping.ipynb`: Main notebook containing all code and explanations.
- `README.md`: This file.

## References

- [Ultralytics Notebooks](https://github.com/ultralytics/notebooks)
- [LangChain Google GenAI](https://python.langchain.com/docs/integrations/chat/google_genai/)

## Notes

- The prototype currently works with static images. Future work may include extracting tabs from videos.
- The accuracy of tab extraction depends on the quality of the input image and the capabilities of the