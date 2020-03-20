# Pandemic Advice from an AI
Just a simple website displaying some questionable public safety announcements
generated using OpenAI's GPT-2.

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