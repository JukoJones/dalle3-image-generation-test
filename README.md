# DALL·E 3 Image Generation Test
---
[Open AI Image Generation Docs](https://platform.openai.com/docs/guides/images/image-generation)

## Notes
---
* Use Colab for best results.
* An Open AI API key to required to use this notebook.
* When using DALL·E 3, images can have a size of 1024x1024, 1024x1792 or 1792x1024 pixels.
* DALL·E 3 Quality Settings: "hd" for enhanced detail.
* Square, standard quality images are the fastest to generate.

## Some Take Aways
---
* You are only able to render one image at a time.
* There is no way to seed this model at the moment or feed a previous image into it. That means that fine-tuning the model is not possible.
* Each generation of an image creates a new prompt on the backend. Even if you don't change any parameters, the model will create a newly generated token string and then generate the image from that.
