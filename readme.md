# Code and Data for "Analyzing Images of Legal Documents: Toward Multi-Modal LLMs for Access to Justice"

This repository contains the code and data for the paper "Analyzing Images of Legal Documents: Toward Multi-Modal LLMs for Access to Justice", accepted at the AI for Access to Justice Workshop at JURIX 2024.

To run this project, you need to provide your own OpenAI API keys. To do so, rename .env-example to .env, and add your OpenAI key. Then, set up a new python environment, install the requirements.txt file, and start a jupyter notebook server to run analyze.ipynb.

The code in analyze.ipynb loads the images from the images folder, and then uses GPT-4o to extract structured data from the images. The results are exported to a file that can be further analyzed. The gold standard data is provided in gold_values.tsv.

If you use the code or data, please cite us at:
```
@inproceedings{westermann2024analyzingimages,
      title={Analyzing Images of Legal Documents: Toward Multi-Modal LLMs for Access to Justice}, 
      author={Hannes Westermann and Jaromir Savelka},
      year={2024},
      booktitle={AI for Access to Justice Workshop at JURIX 2024},
}
```

The forms used in this project are © King's Printer for Ontario, 2020.

# Paper Abstract:
Interacting with the legal system and the government requires the assembly and analysis of various pieces of information that can be spread across different (paper) documents, such as forms, certificates and contracts (e.g. leases). This information is required in order to understand one's legal rights, as well as to fill out forms to file claims in court or obtain government benefits. However, finding the right information, locating the correct forms and filling them out can be challenging for laypeople. Large language models (LLMs) have emerged as a powerful technology that has the potential to address this gap, but still relies on the user to provide the correct information, which may be challenging and error-prone if the information is only available in complex paper documents. We present an investigation into utilizing multi-modal LLMs to analyze images of handwritten paper forms, in order to automatically extract relevant information in a structured format. Our initial results are promising, but reveal some limitations (e.g., when the image quality is low). Our work demonstrates the potential of integrating multi-modal LLMs to support laypeople and self-represented litigants in finding and assembling relevant information.