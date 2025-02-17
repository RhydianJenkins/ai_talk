## Breaking News!

New AI <span data-fragment-index="1" class="fragment highlight-red">model</span>
Deepseek<span data-fragment-index="2" class="fragment highlight-red">-r1</span>
was <span data-fragment-index="3" class="fragment highlight-red">trained</span>
on openAI <span data-fragment-index="4" class="fragment highlight-red">data</span>
and has <span data-fragment-index="6" class="fragment highlight-red">only</span>
<span data-fragment-index="5" class="fragment highlight-red">1.5 billion parameters</span>!

---
## In this talk
<p class="fragment fade-in-then-out">Reasoning models (LLMs that have a 'thinking' stage)</p>
<p class="fragment fade-in-then-out">Transformer models ('Vanilla' LLMs)</p>
<p class="fragment fade-in-then-out">Diffusion models (generating images from noise)</p>
<p class="fragment fade-in-then-out">Convolutional Neural Networks (CNNs)</p>

<div class="fragment" style="position: absolute; top: 60px">
    <p>Multilayer Perceptrons (MLP)</p>
    <img src="/img/MLP.png" height="700" width="1200" />
</div>

---
## Disclaimer

<ul>
    <li>We don't really need to understand this stuff</li>
    <li>This is a heavily simplified explaination</li>
</ul>
<img src="/img/how_to_talk_to_women.png" height="700" width="1200" />

---
## Problem

I want to predict if someone is going to be happy

<img src="/img/happy_or_not.png" height="700" width="700" />

---
## Perceptron

<img src="/img/perceptron.png" />

---
## Perceptron

<img src="/img/formal_perceptron.png" />

[McCulloch & Pitts, 1943](https://www.cse.chalmers.se/~coquand/AUTOMATA/mcp.pdf)

---
## Perceptron

<img src="/img/modern_perceptron.png" />

---
## Multilayer Perceptron (MLP)

<img src="/img/excallidraw_mlp.png" />

---
## Model Training data

```csv
name, age, step count, ..., happiness
Alice, 25, 7000, ..., 0.8
Bob, 34, 12000, ..., 0.9
Charlie, 29, 5000, ..., 0.6
David, 40, 8000, ..., 0.7
Emma, 22, 15000, ..., 0.95
...

```

### Backpropagation Algorithm

- Initialise all weights to random
- Feed in Alice
- If the output is too low, adjust weights the smallest amount you can to move the result up (visa versa)
- Repeat with entire training data set

---
## Timeline

- **1943** – [McCulloch & Pitts proposed the first artificial neuron](https://www.cse.chalmers.se/~coquand/AUTOMATA/mcp.pdf)
- **1957** – [The Perceptron, a single-layer model](https://bpb-us-e2.wpmucdn.com/websites.umass.edu/dist/a/27637/files/2016/03/rosenblatt-1957.pdf)
- **1960s** – Early versions of MLPs were explored, but training was difficult.
- **1986** – [Rumelhart, Hinton, and Williams popularized backpropagation training](https://www.nature.com/articles/323533a0)
- **...**
- **2013** – ['Efficient Estimation of Word Representations in Vector Space' by a Google team](https://arxiv.org/abs/1301.3781)
- **2017** – ['Attention is All You Need' by a Google team](https://arxiv.org/abs/1706.03762)
- **2018** - [Initial GPT paper by OpenAI](https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf)

---
## Fast Forward: LLMs

- Takes **n** input 'tokens' (like 'words')
- Ends up in an 'Embedding space'
- Tokens near that destination are the 'most likely' next token
