# LSTMProteinClassification

Hi There! 👋<br/>
This is a repo where you have access to all the Jupiter Notebooks, along with some resources that made it all possible!<br/>

## Table of Contents
* [What are LSTMs?](#What-are-LSTMs?)
* [What's the Big Deal with Protien Folding?](#What's-the-Big-Deal-with-Protien-Folding?)
* [Acknowledgements](#Acknowledgements)
* [Connect with me](#Connect-with-me)

## What are LSTMs?

### TL;DR 
A chain of little cells blocks that process and pass on information to one another. 

### A Longer Explanation:
LSTMs were originally proposed by Sepp Hochreiter and Jurgen Schmidhuber way back in 1997 in their paper: [Long Short-Term Memory](https://www.bioinf.jku.at/publications/older/2604.pdf). It's an incredible algorithm that's an improved version of Recurrent Neural Networks (RNNs). But let's actually get into what they actually do.

Let's say you wanted to use an algorithm that predicted the next word that you were going to say - What requirements would you need in a system that could do that? First you need to know the context of the sentence, thus you need to know what was said before. In addition you want this to be a continuous process, so you'll be predicting the next word again and again. 

Now let me introduce you to LSTMs:

<p align="center">
<img src="LSTM3-chain.png" width="350"/><br/>
Credit: Christopher Olah
</p>

The x things at the bottom represent the inputs, while the h things at the top represent the outputs. So you put in a word, and the cell spits out an output, or prediction of the next word. But what's important is that these cell blocks are connected with each other! Now they have memory - which allows them to remember the context of sentences.

For my protein classification I my h's (hidden's) weren't predicting the next amino acid, rather they were producing latent factors. Then you take all of the hiddens and you pass them into linear layers (along with some batch norms and sigmoids) and Voila!

## What's the Big Deal with Protien Function Prediction?
A HUGE deal. Every year, the price of genome sequencing is drops as a result of technological process. This is followed by the increase in the number of genomes sequenced. That's awesome. But the problem is: We don't know waht those sequences do. For humans, we still don't understnad 20% of our protein encoding genes! For other species it's far far less.

Those proteins are actually hidden gems that we can harvest. Drug design. Cure to diseases. Manufacturing of valuable substances. Increased understanding of the universe.

I actually wrote a whole [Article](https://dickson-wu.medium.com/unlocking-the-secrets-of-our-genome-with-lstms-636c0724a9f3) about this! Check it out! Also check out my [Video](https://youtu.be/3-Yk3YBqMzU)!

## Acknowledgements

* [Understanding LSTM Networks by Christopher Olah - A wonderful guide to LSTMs](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)
* [Reserach Paper that details the history, evolution and math of LSTMs](https://arxiv.org/pdf/1909.09586.pdf)
* [Illustrated Guide to LSTM’s and GRU’s: A step by step explanation](https://towardsdatascience.com/illustrated-guide-to-lstms-and-gru-s-a-step-by-step-explanation-44e9eb85bf21)
* [The Dataset I used](https://www.kaggle.com/shahir/protein-data-set/notebooks)
* [Resource that helped me code](https://towardsdatascience.com/lstm-text-classification-using-pytorch-2c6c657f8fc0)
* [Resource that helped me code](https://www.analyticsvidhya.com/blog/2020/01/first-text-classification-in-pytorch/)
* [Resource that helped me code](https://huggingface.co/Rostlab/prot_bert)
* [Resource that explains the importance](https://arxiv.org/ftp/arxiv/papers/1701/1701.08318.pdf)
* [Resource that explains the importance](https://www.nature.com/articles/nrm2281)
* [Resource that explains the importance](https://www.newscientist.com/article/2194516-we-dont-know-what-a-fifth-of-our-genes-do-and-wont-find-out-soon/)
* [Resource that explains the importance](https://news.mit.edu/2019/machine-learning-amino-acids-protein-function-0322)
* [Resource that explains the importance](https://www.frontiersin.org/articles/10.3389/fbioe.2020.00391/full)

## Connect with me

If you want to follow along on my journey, you can join my [monthly newsletter](https://www.subscribepage.com/g1p8w4), check out my [website](https://dicksonwu654.github.io/), and connect on [Linkedin](https://www.linkedin.com/in/real-dickson-wu/) or [Twitter](https://twitter.com/DicksonWu3) 😃
