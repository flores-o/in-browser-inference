**Repository: ONNX Runtime Web Inference**

**Description:**
This repository provides an example of performing inference using a pre-trained DistilBERT model fine-tuned for sentiment analysis using ONNX Runtime in a web environment. The model is converted to the ONNX format for inference in a web browser. The web page allows users to input text, and the model predicts the sentiment (positive or negative) of the text.

**Contents:**

- **index.html:** This HTML file contains the web interface for the sentiment analysis model. It includes JavaScript code that loads the ONNX model, tokenizes input text, performs inference, and displays the predicted sentiment and inference time on the web page.

- **convert_to_onnx.ipynb:** This Jupyter Notebook demonstrates how to convert a pre-trained DistilBERT model for sequence classification into ONNX format. It loads a pre-trained DistilBERT model and tokenizer, performs inference on an example text, and exports the model to the ONNX format for use in the web application.

- **models/:** This directory contains the converted ONNX model (`distilbert.onnx`) generated using the custom conversion script, as well as the quantized model (`model_quantized`) provided by [Hugging Face](https://huggingface.co/Xenova/distilbert-base-uncased-finetuned-sst-2-english/tree/main).

- **package.json, package-lock.json:** These files manage the dependencies required for the web application.



**Running the demo:**

``` 
npm install -g http-server
http-server -p 8081 --cors
```



