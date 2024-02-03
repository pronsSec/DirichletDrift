# DirichletDrift 🧵

A robust tool for analyzing and categorizing large datasets using Latent Dirichlet Allocation (LDA).

![image](https://github.com/pronsSec/DirichletDrift/assets/93559326/e5246285-ae33-4a17-b4c6-e66ca3517b7e)










## Introduction

DirichletDrift is a one stop bulk file handling shop. Sorting, indexing, and visualization of relationships all in one! 

It sifts through your file names and leverages LDA to categorize them into distinct topics. Whether you're diving into a fresh unstructured dataset or revisiting a previous one, DirichletDrift provides a one-stop solution to analyze and make sense of your data. By using LDA on your filenames you are able to provide a more in-depth search than just basic keyword searches, potentially unveiling unseen relationships between files. In a large unstructured pile of documents this can make all of the difference!

## Why use this over OS native options?

This tool is best used in a command line environment, I personally use it on my servers where I store bulk unstructured data. It may seem redundant to GUI based file search that is native in all OS's , but speed is the benefit you receive. The framework consolidates multiple tasks. It processes once and then stores your results, making it much quicker than OS native search. 

While LDA on filenames won't delve into the content as deeply as it would on full documents, it still provides a more nuanced understanding than basic keyword searches. By analyzing patterns and themes in filenames, Dirichlet Drift can help categorize and understand files in a way that goes beyond simple name-based searches. This can be particularly useful in scenarios where filenames are descriptive and structured, allowing the LDA to pick up on underlying themes or categorizations that might not be immediately apparent.

And don't forget... speed! LDA on only the filenames provides for lightning fast indexing, that only needs to be done once!

### Deep Content Analysis with LDA:

LDA doesn't just search for filenames or content based on keyword matching. Instead, it analyzes the underlying topics in text-based files, revealing hidden patterns and themes. This is particularly useful for large datasets where content understanding is as important as content finding.


## Features
- 🗂️ Sort and gather files by type from your unsorted files. Neatly Pack into one directory.
- 📊 Perform LDA analysis on file names.
- 🗂️ Create a CSV flat file database for easy examination.
- 🚀 Quick file retrieval based on topics of interest.
- 🎨 Visualize topic distributions with an interactive HTML dashboard output.

## Getting Started

**Clone the Repository**
   ```bash
   git clone https://github.com/pronsSec/DirichletDrift.git &&
   sudo chmod -R 777 DirichletDrift &&
   cd DirichletDrift
```

**Run TopicTapestry**
```
python dirichlet_drift.py
```


---

## Usage

- **Sort and Gather Files**

Use the sort option to recursively sort files by filetype from your system. 

This copies them to a bulk target directory. The LDA script takes only a bulk directory as input, no subdirectories. So, this creates a clean bucket for the LDA script to run on. 
I use this script on massive datasets, and love it. It allows me to bucket unmanageable datasets into neat buckets. Then proceed to topic model them using LDA in steps 2-3. Analyze terabytes like they are putty in your hand. 


- **Perform LDA Analysis**

Upon running runner.py, select the option to perform LDA analysis. (This is not a recursive tool, use the sorting tool to make a bucket to feed it)
The script will guide you through the process. If you used the sorting script feed it that bucket directory you created.


- **Query prior Results**

Opt to query an existing CSV file.
Enter the topic words of interest.
Access the relevant files directly through the tool. Quickly open and read related files. 

- **Access The Interactive HTML Topic Modelling Output Dashboard**

Choose the option for this and the dashboard will open in browser. 

---


*Requirements
All required packages are listed in requirements.txt. TopicTapestry will handle the installation for you.*
