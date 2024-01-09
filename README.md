### Text-To-Image (Bagan Ai Generated)
### Results
  All our results are based on fine-tuning https://huggingface.co/runwayml/stable-diffusion-v1-5 model.

  We display the results using a range of training samples and images from different image categories, such as pagodas and Buddha statues.
  ![Screenshot 2023-10-12 165137](https://github.com/simbolo-ai/Text-to-Image/assets/106800189/fa92aaf2-0346-4563-8d59-17c73440638e)
### Ai Generated Bagan Images:
![ananda bagan](https://github.com/simbolo-ai/Text-to-Image/assets/106800189/6965b965-73ec-436e-9210-5da550b1fe5b) ![download (2)](https://github.com/simbolo-ai/Text-to-Image/assets/106800189/b1b9af8e-5346-4b52-aa64-2f5839efa9c4)

In order to get those images, we trained over 223 General Bagan Images and 137 Ananda Pagodas.

### Problem Statement:
When we prompted the stable diffusion model to generate an image of Bagan, it produced an image depicting a pagoda from Thailand. Hence, our decision was to fine-tune the current stable diffusion model using a multitude of Bagan photos in order to attain a clearer outcome.

### How to use:
prompt = "fantasy bagan,hypper detailed , peaceful mood ,The central theme could revolve around a fantastical journey through a magical realm, featuring characters with ethereal and surreal qualities, set against a backdrop of vibrant and enchanting landscapes, The color palette would be a harmonious combination of  Jean's bold and surreal hues, by yukisakura  sunset."
negative_prompt = ""
num_samples = 5 
guidance_scale = 9
num_inference_steps = 100 
height = 512
width = 512 

with autocast("cuda"), torch.inference_mode():
    images = pipe(
        prompt,
        height=height,
        width=width,
        negative_prompt=negative_prompt,
        num_images_per_prompt=num_samples,
        num_inference_steps=num_inference_steps,
        guidance_scale=guidance_scale,
        generator=g_cuda
    ).images

for img in images:
    display(img)

### Data:
We used stable diffusion v1.5 model to train with 223 bagan pictures.

### Contributors:
Main Contributor: Ye Bhone Lin ![https://github.com/Ye-Bhone-Lin], Supervisor: 

  
