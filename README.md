<p align="center">
    <br>
    <img src="https://s3.amazonaws.com/ps.public.resources/ml-showcase/ml-showcase-header.png" width="400"/>
    <br>
<p>
<p align="center">
    <a href="https://github.com/gradient-ai/aitextgen/blob/master/LICENSE">
        <img alt="GitHub" src="https://img.shields.io/github/license/gradient-ai/aitextgen.svg?color=blue">
    </a>
    <a href="https://github.com/gradient-ai/aitextgen">
        <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/gradient-ai/aitextgen">
    </a>
    <a href="https://console.paperspace.com/github/gradient-ai/aitextgen">
        <img src="https://assets.paperspace.io/img/gradient-badge.svg" alt="Run on Gradient"/>
    </a>
</p>
<hr />
<h1 align="center">
    aitextgen
</h1>

This is a fork of [aitextgen](https://github.com/minimaxir/aitextgen) notebooks by [Max Woolf](https://github.com/minimaxir). 

This repository makes a number of demo notebooks available for use in Paperspace Gradient:
|Notebook|Run on Gradient Link|
|---|---|
|Train a GPT-2 model + tokenizer from scratch (GPU)|[![Gradient](https://assets.paperspace.io/img/gradient-badge.svg)](https://console.paperspace.com/github/gradient-ai/aitextgen/blob/master/aitextgen_—%C2%A0Train_a_Custom_GPT_2_Model_%2B_Tokenizer.ipynb)|
|Finetune OpenAI's 124M GPT-2 model (or GPT Neo) on your own dataset (GPU)|[![Gradient](https://assets.paperspace.io/img/gradient-badge.svg)](https://console.paperspace.com/github/gradient-ai/aitextgen/blob/master/aitextgen_—_Train_a_GPT_2_(or_GPT_Neo)_Text_Generating_Model_w_GPU.ipynb)|
|aitextgen Generation Hello World|[![Gradient](https://assets.paperspace.io/img/gradient-badge.svg)](https://console.paperspace.com/github/gradient-ai/aitextgen/blob/master/generation_hello_world.ipynb)|
|aitextgen Training Hello World|[![Gradient](https://assets.paperspace.io/img/gradient-badge.svg)](https://console.paperspace.com/github/gradient-ai/aitextgen/blob/master/training_hello_world.ipynb)|
|Hacker News aitextgen|[![Gradient](https://assets.paperspace.io/img/gradient-badge.svg)](https://console.paperspace.com/github/gradient-ai/aitextgen/blob/master/hacker_news_demo.ipynb)|
|Reddit aitextgen|[![Gradient](https://assets.paperspace.io/img/gradient-badge.svg)](https://console.paperspace.com/github/gradient-ai/aitextgen/blob/master/reddit_demo.ipynb)|


## Description

aitextgen is a robust Python tool for text-based AI training and generation using [OpenAI's](https://openai.com) [GPT-2](https://openai.com/blog/better-language-models/) and [EleutherAI's](https://www.eleuther.ai) [GPT Neo/GPT-3](https://github.com/EleutherAI/gpt-neo) architecture.

aitextgen is a Python package that leverages [PyTorch](https://pytorch.org), [Hugging Face Transformers](https://github.com/huggingface/transformers) and [pytorch-lightning](https://github.com/PyTorchLightning/pytorch-lightning) with specific optimizations for text generation using GPT-2, plus _many_ added features. It is the successor to [textgenrnn](https://github.com/minimaxir/textgenrnn) and [gpt-2-simple](https://github.com/minimaxir/gpt-2-simple), taking the best of both packages:

- Finetunes on a pretrained 124M/355M/774M GPT-2 model from OpenAI or a 125M/350M GPT Neo model from EleutherAI...or create your own GPT-2/GPT Neo model + tokenizer and train from scratch!
- Generates text faster than gpt-2-simple and with better memory efficiency!
- With Transformers, aitextgen preserves compatibility with the base package, allowing you to use the model for other NLP tasks, download custom GPT-2 models from the HuggingFace model repository, and upload your own models! Also, it uses the included `generate()` function to allow a massive amount of control over the generated text.
- With pytorch-lightning, aitextgen trains models not just on CPUs and GPUs, but also _multiple_ GPUs and (eventually) TPUs! It also includes a pretty training progress bar, with the ability to add optional loggers.
- The input dataset is its own object, allowing you to not only easily encode megabytes of data in seconds, cache, and compress it on a local computer before transporting to a remote server, but you are able to _merge_ datasets without biasing the resulting dataset, or _cross-train_ on multiple datasets to create blended output.


## Tags
<code>NLP</code>, <code>GPT-2</code>, <code>Educational</code>



## Launching Notebook
By clicking the <code>Run on Gradient</code> button above, you will be launching the contents of this repository into a Jupyter notebook on Paperspace Gradient. 


## Docs
Docs are available at docs.paperspace.com. 

Be sure to read about how to <a href="https://docs.paperspace.com/gradient/notebooks/create-a-notebook">create a notebook</a> or <a href="https://youtu.be/i4pvLzvw2ME">watch the video</a> instead!
