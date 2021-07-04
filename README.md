# GPT-Code-Clippy (GPT-CC)

# Open Source GitHub Copilot for auto generating code

I would like to train an open source version of the new awesome GitHub Copilot AI tool, which is based on GPT3. Similar to the awesome people behind GPT-Neo, having such an open source model would greatly help researchers understand what this type of biases and limitations this kind of code autocompletion model might have such as generating insecure code (i do research in this area and i know my team would love an open sourced version to run experiments on, i.e. try and break it 🤓)

## 2. Language

The model will be trained on different programming languages such as C, C++, java, python, etc.

## 3. Model

GPT-Neo

## 4. Datasets

Datasets that contain hopefully high quality source code

Possible links to publicly available datasets include:
- https://huggingface.co/datasets/code_search_net
- https://huggingface.co/datasets?search=code_x

Some additional datasets may need creating that are not just method level.

## 5. Training scripts

I believe the standard CLM language model script would do for this.

We can make use of https://www.github.com/huggingface/transformers/tree/master/examples%2Fflax%2Flanguage-modeling%2Frun_clm_flax.py

## 6. (Optional) Challenges

The data additional data may be a challenge. From what I can see in copilot, it looks to be training on entire files, not code snippets. There are file level datasets that exist but they are a few years old and i don't think they cover many programming languages. The ones I listed above have multiple languages but are only methods.

However, githubs API is pretty easy to use and so it would be pretty easy to create one from scratch, especially if we get some insights into how the copilot dataset was generated 🤓

## 7. (Optional) Desired project outcome

I'd love to have this open source model setup in a similar Visual Studio Code extension to the GitHub Copilot one. I've actually made a tutorial on doing this using the GPT-Neo model, so we could easily clean it up and release it free of charge forever because from what I've seen on Twitter the GitHub Copilot might eventually be put behind a paywall 😢.

## 8. (Optional) Reads

The following links can be useful to better understand the project and 
what has previously been done.

- https://github.blog/2021-06-29-introducing-github-copilot-ai-pair-programmer/
- https://youtu.be/nC3NrhoNeP4  (tutorial on how we could setup the demo of the model once it's done cooking)