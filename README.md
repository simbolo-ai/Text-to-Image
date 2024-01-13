### Text-To-Image (Bagan Ai Generated)
### Results
  All our results are based on fine-tuning https://huggingface.co/runwayml/stable-diffusion-v1-5 model.

  We display the results using a range of training samples and images from different image categories, such as pagodas and Buddha statues.
  ![Screenshot 2023-10-12 165137](https://github.com/simbolo-ai/Text-to-Image/assets/106800189/fa92aaf2-0346-4563-8d59-17c73440638e)
### Ai Generated Bagan Images:
![ananda bagan](https://github.com/simbolo-ai/Text-to-Image/assets/106800189/6965b965-73ec-436e-9210-5da550b1fe5b) ![download (2)](https://github.com/simbolo-ai/Text-to-Image/assets/106800189/b1b9af8e-5346-4b52-aa64-2f5839efa9c4)

In order to get those images, we trained over 223 General Bagan Images and 137 Ananda Pagodas.

### Introduction:
Meet General Bagan, a cutting-edge text-to-image generator trained on a diverse dataset of over 200 images. With a keen understanding of textual inputs, it effortlessly translates words into visually stunning representations. From lifelike nature scenes to captivating abstract compositions.

### Problem Statement:
When we prompted the stable diffusion model to generate an image of Bagan, it produced an image depicting a pagoda from Thailand. Hence, our decision was to fine-tune the current stable diffusion model using a multitude of Bagan photos in order to attain a clearer outcome.

### How to create prompt:
When we create prompt for bagan, we have to consider 6 keywords. Those are Subject, Medium, Style, Art-sharing website, Resolution, and Additional details. 
Subject -> What you want to see in the picture is the subject. Not writing enough about the subjects is a common error.
Medium -> The medium is the substance that artists work with. Illustration, oil painting, 3D rendering, and photography are a few examples. The impact of Medium is significant because a single keyword can significantly alter the style.
Style -> The image's artistic style is referred to as the style. Pop art, impressionist, and surrealist are a few examples.
Art-sharing website -> Specialty graphic websites like Deviant Art and Artstation compile a large number of images from various genres. One surefire way to direct the image toward these styles is to use them as a prompt.
Resolution -> Resolution represents how sharp and detailed the image is
Additional Details -> Sweeteners added to an image are additional details. To give the image a more dystopian and sci-fi feel, we will add those elements.
The example prompt for general bagan is: bagan, a creepy and eery Halloween setting, with Jack o lanterns on the street and shadow figures lurking about, dynamic lighting, photorealistic fantasy concept art, stunning visuals, creative, cinematic, ultra detailed, trending on art station, spooky vibe.
That prompt gives you the Halloween theme.

### Data:
We used stable diffusion v1.5 model to train with 223 bagan pictures.

### Contributors:
Main Contributor: [Ye Bhone Lin](https://github.com/Ye-Bhone-Lin), Supervisor: Sa Phyo Thu Htet, Contributors: Thant Htoo San, Min Phone Thit

### Limitation:
We can't generate a photo of a human.

### References:
Wikipedia (2022). Stable Diffusion. Retrieved From: https://en.wikipedia.org/wiki/Stable_Diffusion

Rombach, R., Blattmann, A., Lorenz, D., Esser, P., & Ommer, B. (2022). High-Resolution Image Synthesis with Latent Diffusion Models. Retrieved From: https://arxiv.org/abs/2112.10752

Naomi Brown (2022). What is Stable Diffusion and How to Use it. Retrieved From: https://www.fotor.com/blog/what-is-stable-diffusion

Mishra, O. (June, 9). Stable Diffusion Explained. Medium. https://medium.com/@onkarmishra/stable-diffusion-explained-1f101284484d

