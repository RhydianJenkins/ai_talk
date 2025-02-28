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

<section>
    <h4>Multilayer Perceptron (MLP)</h4>
    <img src="/img/excallidraw_mlp.png" />
</section>

<section>
    New AI <span data-fragment-index="1" class="fragment highlight-red">model</span>
    Deepseek<span data-fragment-index="2" class="fragment highlight-red">-r1</span>
    was <span data-fragment-index="3" class="fragment highlight-red">trained</span>
    on openAI <span data-fragment-index="4" class="fragment highlight-red">data</span>
    and has <span data-fragment-index="6" class="fragment highlight-red">only</span>
    <span data-fragment-index="5" class="fragment highlight-red">1.5 billion parameters</span>!
</section>

---
## Model Training data

```
name, age, step count, ..., happiness
Alice, 25, 7000, ..., 0.8
Bob, 34, 12000, ..., 0.9
Charlie, 29, 5000, ..., 0.6
David, 40, 8000, ..., 0.7
Emma, 22, 15000, ..., 0.95
...
// and many more...

```

### Backpropagation Algorithm

```txt
1. Initialise all weights to random
2. Feed in Alice (called 'Feed Forward')
3. Adjust weights to improve result
4. Repeat with entire training data set
```

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
## LLMs; What do they do?

<div style="position: relative; height: 2em;">
  <div class="fragment fade-out" style="position: absolute; width: 100%;">Once upon a...</div>
  <div class="fragment fade-in-then-out" style="position: absolute; width: 100%;">Once upon a time...</div>
  <div class="fragment fade-in-then-out" style="position: absolute; width: 100%;">Once upon a time there...</div>
  <div class="fragment fade-in-then-out" style="position: absolute; width: 100%;">Once upon a time there lived...</div>
  <div class="fragment fade-in-then-out" style="position: absolute; width: 100%;">Once upon a time there lived a...</div>
</div>

<img src="/img/llm_input_example.png" />

---

```txt
System: You are a helpful AI that answers user questions
User question: What is the best way to cook an egg?
System: ...
```

<img src="/img/llm_input_example_2.png" />

---

<img src="/img/transformer_architecture.png" />

---

<img src="/img/llm_diagram_simple.png" />

---
## Feed Forward

<img src="/img/excallidraw_mlp.png" />

---

<img src="/img/embedding_1.png" />

---

<img src="/img/embedding_2.png" />

---

<img src="/img/embedding_examples.png" />

['Efficient Estimation of Word Representations in Vector Space' by a Google team, 2013](https://arxiv.org/abs/1301.3781)

---

<img src="/img/embedding_3.png" />

---
## Attention?

"She turned on the <span data-fragment-index="1" class="fragment highlight-red">light</span> to brighten the room"

"The bag was surprisingly <span data-fragment-index="2" class="fragment highlight-red">light</span>, so carrying it was easy"

"He tried to keep the conversation <span data-fragment-index="3" class="fragment highlight-red">light</span> to avoid tension"

---

<p style="text-align: left">
    The poker game was tense. Eddie "Ace" Malone laid down four kings, smirking. Vincent Russo’s face darkened. He had lost everything. "You cheated," Vincent growled.
    Eddie laughed.
</p>
<p style="font-style: italic;">
    10,000 words later...
</p>
<p style="text-align: left">
    A shot rang out. Eddie slumped forward, blood pooling on the table. Don't ever cheat again, said <span class="fragment" style="color: red;">?</span>
</p>

---

## End

New AI model Deepseek-r1 was trained on openAI data and has only 1.5 billion parameters

