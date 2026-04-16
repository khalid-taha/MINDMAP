## Prompt to create a mind map from text

Read the text and turn it into a **mind map based only on keywords and relationships found in the text**.

### Your job

Do these steps in order:

### 1. Identify the keywords

Extract the most important meaning-carrying words and short phrases from the text.

A **keyword** can be:

* a main noun
* a main verb
* a key adjective
* a short phrase that carries one clear idea

Do **not** limit keywords to nouns only.

Include words like:

* actions: **trained, uses, learn, generate, predict**
* concepts: **LLM, transformer architecture, parameters, context**
* key phrases: **massive amounts of text data, predicting the next word in a sequence**

Do **not** include weak filler words unless they are clearly part of the relationship in the source text.

Avoid:

* articles and filler words such as **the, a, an, very**
* generic connector words that add no meaning on their own
* invented words not present in the source text
* long sentences copied from the source

### 2. Identify the relationships between the keywords

Find how the keywords connect to each other in the source text.

A relationship should show:

* what something **is**
* what something **does**
* what something **uses**
* what something **is trained on**
* what something **allows**
* what something **includes**
* what something **belongs to**
* cause, result, part-whole, hierarchy, or function

The relationship words should come from the source text where possible.

Do not invent new ideas.

### 3. Build the mind map

Create a tree-style mind map.

Rules:

* Put the main topic at the top
* Group related keywords together
* Show the relationship by the structure of the tree
* Keep each node short
* Use only keywords and relationship words taken from, or directly justified by, the text
* Do not add explanation outside the map unless asked

### 4. Output in this format

For each text, produce:

**Keywords**
[list of keywords]

**Relationships**

* keyword → relationship → keyword
* keyword → relationship → keyword

**Mind map**
Tree layout using this style:

**Main Topic**
├── **keyword / relationship**
│   └── **keyword**
└── **keyword / relationship**
└── **keyword**

### Important rules

* A keyword is not only a noun. It can also be a main verb or a key phrase.
* Keep the map faithful to the source text.
* Do not make the map too thin by dropping important action words.
* Do not make the map too dense by copying whole sentences.
* If a relationship is important in the text, include it.
* If a word is central to meaning, keep it even if it is a verb.
* Prefer short phrases over single words when the phrase carries the real meaning.
* Do not add outside knowledge.
* Do not paraphrase heavily.
* Do not use vague labels such as “thing”, “stuff”, “aspect”, or “details”.

---

## Example 1

### Input text

An LLM is a deep neural network trained on massive amounts of text data to understand, generate, and respond to human-like text. It uses a transformer architecture to pay attention to different parts of the input, making it adept at handling language nuances. LLMs are trained on the task of predicting the next word in a sequence, which allows them to learn context, structure, and relationships within text.

### Output

**Keywords**
LLM, deep neural network, trained, massive amounts of text data, understand, generate, respond, human-like text, uses, transformer architecture, pay attention, different parts of the input, adept, handling language nuances, predicting the next word in a sequence, allows, learn, context, structure, relationships within text

**Relationships**

* LLM → deep neural network
* LLM → trained → massive amounts of text data
* LLM → understand → human-like text
* LLM → generate → human-like text
* LLM → respond → human-like text
* LLM → uses → transformer architecture
* transformer architecture → pay attention → different parts of the input
* pay attention → adept → handling language nuances
* LLMs → trained → predicting the next word in a sequence
* predicting the next word in a sequence → allows → learn
* learn → context
* learn → structure
* learn → relationships within text

**Mind map**
**LLM**
├── **deep neural network**
├── **trained**
│   ├── **massive amounts of text data**
│   └── **predicting the next word in a sequence**
│       └── **allows**
│           └── **learn**
│               ├── **context**
│               ├── **structure**
│               └── **relationships within text**
├── **understand**
│   └── **human-like text**
├── **generate**
│   └── **human-like text**
├── **respond**
│   └── **human-like text**
└── **uses**
└── **transformer architecture**
└── **pay attention**
└── **different parts of the input**
└── **adept**
└── **handling language nuances**

---

## Example 2

### Input text

Traditional machine learning requires manual feature extraction, where human experts identify and select relevant features for the model. Deep learning, on the other hand, does not require this manual process, allowing the model to learn features directly from the data.

### Output

**Keywords**
traditional machine learning, requires, manual feature extraction, human experts, identify, select, relevant features, model, deep learning, does not require, manual process, allowing, learn features, directly from the data

**Relationships**

* traditional machine learning → requires → manual feature extraction
* human experts → identify → relevant features
* human experts → select → relevant features
* relevant features → model
* deep learning → does not require → manual process
* deep learning → allowing → learn features
* learn features → directly from the data

**Mind map**
**traditional machine learning**
├── **requires**
│   └── **manual feature extraction**
├── **human experts**
│   ├── **identify**
│   │   └── **relevant features**
│   └── **select**
│       └── **relevant features**
└── **model**
└── **relevant features**

**deep learning**
├── **does not require**
│   └── **manual process**
└── **allowing**
└── **learn features**
└── **directly from the data**

---

