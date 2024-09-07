## Count Anything in Large-Scale Unlabeled Datasets

Counting items of interest in large-scale image collections is important to various fields, such as ecology and history, as it supports essential quantitative analyses. Traditional methods depend on domain-specific detectors and extensive labeled data, while Vision-Language Models (VLMs), like OpenAI's CLIP, offer a more flexible, query-based approach. Most VLMs, however, do not perform well on this task out-of-the-box, with fine-tuning still requiring substantial labeling and computational effort. As an alternative, we apply DISCount to our multimodal setting as a human-in-the-loop approach to produce unbiased count estimates for images that match  queried text within a given dataset. Furthermore, we devise an Adaptive method on top of DISCount that consists of training a logistic regression model on a subset of screened images to iteratively improve the Importance sampling proposal distribution. Our method consistently generates more accurate count estimates when compared to DISCount for increasingly difficult categories of queries when tested on a modified version of the Caltech 256 and the CUB datasets. We also showcase our estimates to have a reduced variance and present experiments and guidelines for choosing hyperparameters for the Adaptive method based on the type of query. While primarily catered towards images and natural language, our method serves as a proof-of-concept for accurate and flexible human-in-the-loop counting in other multimodal contexts with massive unlabeled data. 


<img width="640" alt="Screen Shot 2024-09-07 at 9 17 18 AM" src="https://github.com/user-attachments/assets/37ea498d-f953-4210-9c03-3689ace63398">


[Read the Entire Report Here](count_anything.pdf)
