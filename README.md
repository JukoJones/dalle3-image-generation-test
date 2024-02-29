# DALL·E 3 Image Generation Test
---
[Open AI Image Generation Docs](https://platform.openai.com/docs/guides/images/image-generation)

## Notes
---
* Use Colab for best results.
* An Open AI API key is required to use this notebook.
* Images can have a size of 1024x1024, 1024x1792 or 1792x1024 pixels.
* Quality Settings: "hd" for enhanced detail.
* Square, standard quality images are the fastest to generate.

## Some Take Aways
---
* You are only able to render one image at a time.
* There is no way to seed this model at the moment or feed a previous image into it. That means that fine-tuning the model is not possible.
* Each generation of an image creates a new prompt on the backend. Even if you don't change any parameters, the model will create a newly generated token string and then generate the image from that.

## Conclusion
---
- After some testing, the model won't accept a string of numbers, a list of numbers, or an object of tokens. It throws the security warning each time.
- After trying various aspects of the `DALL·E 3` API, I found that even though you can change the context of the prompt throughout the process, there is no real way to get relaible and repeatable results from the model.
- The rewriting of the prompt with each injection of the prompt doesn't allow for repeatablility.
- The hope is they open this API like they did with `DALL·E 2` to allow for a more iterative approach without altering the state of the prompt with each request.
