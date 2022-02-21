# Paper Title

## Paper Summary
#### What is the paper about? Please, be concise (3 to 5 sentences)
This paper presents an approach to human motion modeling based on convolutional neural networks. In this encoder-decoder approach, a convolutional long term encoder and a short term encoder are used to encode the long term hidden variable and the short term hidden variable. Experiments show better performance on the Human3.6M and CMU Motion Capture datasets.

## Paper methodology
#### Go into detail about the methodology used in the paper

## Paper Strengths
#### Please discuss, justifying your comments with the appropriate level of details, the strengths of the paper (i.e. novelty, theoretical approach and/or technical correctness, adequate evaluation, clarity, etc). For instance, a theoretical paper may need no experiments, while a paper with a new approach may require comparisons to existing methods.
A seeming reasonable approach has been proposed in this paper. Compared to existed methods, this work seems to achieve better results.

## Paper Weaknesses
#### Please discuss, justifying your comments with the appropriate level of details, the weaknesses of the paper (i.e. lack of novelty – given references to prior work-, lack of novelty, technical errors, or/and insufficient evaluation, etc). Note: If you think there is an error in the paper, please explain why it is an error. Also remember that theoretical results/ideas are essential to CVPR (some theoretical papers may not need to have experiments). If the theory is novel and interesting, but the results did not outperform other existing algorithms, it is not necessarily a reason to reject. It is not appropriate to ask for comparisons with unpublished papers and papers published after the CVPR deadline. In all cases, please be polite and constructive. CVPR 2018 policy on dual submission and arxiv appears at: http://cvpr2018.thecvf.com/submission/main_conference/author_guidelines.	However, as to the novelty and the experimental results, I have the concerns as follows:

1.  The authors should demonstrate the roles of long term encoder and short term encoder in the experiments, respectively. The same operations with different sequence length in these two encoders are very weird.

2.  How to verify the effectiveness of the Rect Conv? Why not Rect Conv along the temporal axis which can capture long temporal dependency?

3. It is very strange to take skeleton sequence as two-dimensional map which is encoded by convolutional networks, which should be modelled by a recurrent structure. Moreover, the better experimental results with more tunings cannot demonstrate the advantages of CNN.

4. What is the motivation of this work on motion modelling, just to prove that CNN is much better?

5. Why do not cite much better results from RRNN [15], e.g., 0.27 for walking (80ms) in Table 1?

6. Some typos, e.g., it should be RRNN not RNN in Table 2.

## Preliminary Rating
#### Please rate the paper according to one of the following six choices:
Weak Reject

## Preliminary Evaluation
#### Please indicate to the AC, your fellow reviewers, and the authors your current opinion on the paper. Please tell the ACs what points you think have the most weight in your reviews and summary, and why.
This paper lacks of enough novelty. The effectiveness of the network structure should be verified by more experiments. It is not suitable to be accepted by CVPR.

## Confidence
Very Confident - to stress that you are pretty sure about your conclusions (e.g., you are an expert who works in the paper's area).


## Final Recommendation
#### Please provide your final recommendation by taking into consideration the rebuttal, other reviews and discussions.
Thank the authors for answering the concerns with more facts and explanations, e.g., Rect Conv, motivation and some results of RRNN. I do not like Reviewer_3 to complain more on personal opinions on how to model sequence with CNN or RNN. Actually, I hope to hear more insights from the authors on the problem. Using either CNN or RNN is not the keypoint.

## Final Rating
#### Please rate the paper according to one of the following six choices:
Poster

<!--Source: https://zzhang.org/review/cvpr18.html -->
