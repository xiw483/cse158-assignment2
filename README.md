Tasks
Assignments will be graded based on their coverage of the following five components. Examples of what might
be included in these sections and previous assignment examples shall be described in more detail in class. Each
of the five sections below will contribute approximately 5 percent of your grade, for a total of 25 percent for
the whole assignment.
1. Identify a dataset to study, and perform an exploratory analysis of the data. Describe the dataset,
including its basic statistics and properties, and report any interesting findings. This exploratory analysis
should motivate the design of your model in the following sections. Datasets should be reasonably large
(e.g. more than 50,000 samples).
2. Identify a predictive task that can be studied on this dataset. Describe how you will evaluate your
model at this predictive task, what relevant baselines can be used for comparison, and how you will assess
the validity of your model’s predictions. It’s fine to use models that were described in class here (i.e.,
you don’t have to invent anything new (though you may!)), though you should explain and justify which
model was appropriate for the task. It’s also important in this section to carefully describe what features
you will use and how you had to process the data to obtain them.
3. Describe your model. Explain and justify your decision to use the model you proposed. How will you
optimize it? Did you run into any issues due to scalability, overfitting, etc.? What other models did you
consider for comparison? What were your unsuccessful attempts along the way? What are the strengths
and weaknesses of the different models being compared?
4. Describe literature related to the problem you are studying. If you are using an existing dataset, where
did it come from and how was it used? What other similar datasets have been studied in the past and
how? What are the state-of-the-art methods currently employed to study this type of data? Are the
conclusions from existing work similar to or different from your own findings?
5. Describe your results and conclusions. How well does your model perform compared to alternatives,
and what is the significance of the results? Which feature representations worked well and which do not?
What is the interpretation of your model’s parameters? Why did the proposed model succeed why others
failed (or if it failed, why did it fail)?


# [Goodreads Datasets](https://sites.google.com/eng.ucsd.edu/ucsdbookgraph/home)

The datasets were collected in late 2017 from [goodreads](https://goodreads.com). Details of the datasets are described in the [dataset website](https://sites.google.com/eng.ucsd.edu/ucsdbookgraph/home)

**We collected these datasets for academic use only! Please do not redistribute them or use for commercial purposes.**

## Citations
If you are using our dataset, please cite the following papers:

- Mengting Wan, Julian McAuley, "[Item Recommendation on Monotonic Behavior Chains](https://github.com/MengtingWan/mengtingwan.github.io/raw/master/paper/recsys18_mwan.pdf)", in RecSys'18. [[bibtex](https://dblp.uni-trier.de/rec/bibtex/conf/recsys/WanM18)]
- Mengting Wan, Rishabh Misra, Ndapa Nakashole, Julian McAuley, "[Fine-Grained Spoiler Detection from Large-Scale Review Corpora](https://github.com/MengtingWan/mengtingwan.github.io/raw/master/paper/acl19_mwan.pdf)", in ACL'19. [[bibtex](https://dblp.uni-trier.de/rec/bibtex/conf/acl/WanMNM19)]



## Notebooks/Code Samples

We've created several notebooks (in python 3.7) to illustrate how to download/read these datasets, and provide some basic explorations of the data.

- [download.ipynb](/download.ipynb): If you prefer to download datasets without GUI. This notebook will show how to download files in bash/python. **Note: It requires installing the [gdown](https://github.com/wkentaro/gdown) package as the datasets are hosted on google drive.**
- [samples.ipynb](/samples.ipynb): This notebook will show how to read '.json.gz' files line-by-line and display sample records of each file.
- [statistics.ipynb](/statistics.ipynb): This notebook will calculate some basic statistics of the datasets (except the largest complete interaction file 'goodreads_interactions.csv'). Running this notebook may take a while.
- [distributions.ipynb](/distributions.ipynb): This notebook will operate on the complete interaction file 'goodreads_interactions.csv' and provide some explorations of the distributions of these interactions. **Note: Run this notebook only when you have LARGE memory (recommend 32g+)!!**
- [reviews.ipynb](/reviews.ipynb): This notebook will calculate some statistics of the review datasets.

