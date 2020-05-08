# Questionable Pandemic Advice from an AI
Just a simple website displaying some questionable public safety announcements
generated using OpenAI's GPT-2.  View it
[here](https://averyhiebert.github.io/pandemic-advice/), or read a blog post
about it [here](https://noctes.mathematicae.ca/generating-questionable-pandemic-advice-with-gpt-2.html).

In case it wasn't clear, this advice is mostly bad and you shouldn't follow it.
Also, I can't 100% guarantee that all of the advice is family-friendly.

## How was the advice generated?
I generated the advice using the large GPT-2 model 
(a.k.a. the model that was initially deemed "too dangerous to release" due
to the possibility that it might be used to generate misinformation online).

There was no fine-tuning step; I took the pretrained model, 
primed it with an appropriate context, and asked it to complete the sentence
"In the event of a global pandemic, remember: ".

The context was created by randomly selecting 3 of the following 5 lines:
```
In the event of a global pandemic, remember: Wash hands frequently.
In the event of a global pandemic, remember: Cancel large public gatherings.
In the event of a global pandemic, remember: Disinfect commonly touched surfaces.
In the event of a global pandemic, remember: Avoid touching your face.
In the event of a global pandemic, remember: Observe social distancing.
```

I generated 7,765 unique warnings in this way.

[Link to the generation script.](https://github.com/averyhiebert/generate-things)
