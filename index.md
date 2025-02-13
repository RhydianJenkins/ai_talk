## News just in!

New Deepseek <span class="fragment highlight-red">model</span> is <span class="fragment highlight-red">trained</span> on openAI <span class="fragment highlight-red">data</span> and has <span class="fragment highlight-red">1.5 billion parameters</span>!

---
## In this talk

<p class="fragment fade-out">Transformer Architecture (LLMs)</p>
<p class="fragment fade-out">Diffusion models</p>
<p class="fragment fade-out">Convolutional Neural Networks (CNNs)</p>

<div class="fragment" style="position: absolute; top: 60px">
    <p>Multilayer Perceptrons (MLP)</p>
    <img src="/img/MLP.png" height="700" width="1200" />
</div>


---
## Disclaimer

We don't really need to understand this stuff

We just call OpenAI's API for our features at BaseKit

<img src="/img/how_to_talk_to_women.png" height="700" width="1200" />

---
## Problem

I want to predict if someone is going to be happy

<img src="/img/happy_or_not.png" height="700" width="700" />


---
## Solution Part 1: Perceptron

<img src="/img/perceptron.png" />

---
## Solution Part 1: Perceptron

How happy (`y`) is someone likely to be?

<img src="/img/perceptron_edited.png" />

---
## Solution Part 1: Our Happyness Example

image of perceptron with our happiness inputs

---

### Examples:

- **Does someone own a house?**
  - 'What is their salary?'
  - 'What is their age?'
  - 'Where do they live?'

- **Is it going to rain?**
  - 'Humidity?'
  - 'Time of year?'
  - 'Temperature?'
  - 'Geographical location?'

- Other examples: 'Is someone going to be tall?', 'Will my team win the next World Cup?', 'Are people going to understand this talk?'

---
## Solution Part 2: Multi-Layer Perceptron

- Multi-layer example:
  - **Is someone going to be happy?**
  - Could take the previous weather and house perceptrons and use those to predict the answer.
- Now we take loads of these and tie them together.
- Give a new, more complex example.
- Show how each neuron/perceptron contributes.

---
## Model Training

- We have been manually adjusting the weights of each input to get good results.
- If we knew the desired result, we could use **backpropagation** (a form of training).
- We know if a person is happy, so we can take their inputs and adjust the weights and biases to give the correct result.
  - Start with random weights and biases.
  - Uses the magic of 'math' aka backpropagation.
  - Propagating backwards in a network and adjusting the weights and biases to move closer to the desired output.

---
## Timeline

- **1943** – [McCulloch & Pitts proposed the first artificial neuron](https://www.cse.chalmers.se/~coquand/AUTOMATA/mcp.pdf)
- **1957** – [Rosenblatt introduced the Perceptron, a single-layer model](https://bpb-us-e2.wpmucdn.com/websites.umass.edu/dist/a/27637/files/2016/03/rosenblatt-1957.pdf)
- **1960s** – Early versions of MLPs were explored, but training was difficult.
- **1986** – [Rumelhart, Hinton, and Williams popularized backpropagation, making MLPs effective for learning](https://www.nature.com/articles/323533a0)
- **...**
- **2023** – ["Attention is All You Need" by Google](https://arxiv.org/abs/1706.03762), originally for translating text

---
## Fast Forward: How do LLMs work?

- **High-level overview:**
  - Takes **n** input tokens.
  - Instead of a number response, they predict the next most likely token
