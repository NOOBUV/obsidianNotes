To generate diffused QR codes using a machine learning model, you would organize your dataset into the following folders:

1. **Conditioning Images Folder:** In this folder, you would include images that represent the background or context onto which the QR codes will be diffused. These could be various types of images, such as landscapes, textures, patterns, or any other background you want to diffuse the QR codes onto. The conditioning images provide the visual context for the QR codes.
    
2. **Target Images Folder:** This folder would contain the QR code images that you want to diffuse onto the conditioning images. These QR code images would typically be in a format compatible with your model, such as PNG or JPEG. Each QR code image represents the desired output for the model—how the QR code should appear once diffused onto the conditioning image.
    
3. **Prompt Text Files Folder:** In this folder, you could include text files that provide prompts or instructions to the model regarding how to diffuse the QR codes onto the conditioning images. These prompts could include details about the desired placement of the QR codes, the level of diffusion, any specific styles or effects to apply, or any other guidance relevant to the generation process.
    

With these folders organized in your dataset, you can train a machine learning model to generate images of diffused QR codes by learning from the conditioning images, target QR code images, and any provided prompts. The model would aim to generate images that effectively blend the QR codes into the context provided by the conditioning images while adhering to the given instructions or prompts.
[Trainer](https://github.com/diontimmer/ControlNet-Trainer)
