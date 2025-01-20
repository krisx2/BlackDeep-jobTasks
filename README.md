# BLACKDEEP JOB TASK

- Task1 - llm summary
  
  1. Explained in jupyter notebook↑↑↑↑↑
 
  
  - [with ollama library](https://nbviewer.org/github/krisx2/BlackDeep-jobTasks/blob/main/ollamatask1.ipynb)
  - [with langchain library](https://nbviewer.org/github/krisx2/BlackDeep-jobTasks/blob/main/task1langchain.ipynb)
  
  
- Task2 - Image generation
  1. Prompts Used - **positive prompt** : *a caucasian man in black clothes with brown hair  and a woman with curly black hair and blue eyes,nature,sunset,closeup photo*,

     **negative prompt** :  *(nsfw, naked, nude, deformed iris, deformed pupils, semi-realistic, cgi, 3d, render, sketch, cartoon, drawing, anime, mutated hands and fingers:1.4), (deformed, distorted, disfigured:1.3), poorly drawn, bad anatomy, wrong anatomy, extra limb, missing limb, floating limbs, disconnected limbs, mutation, mutated, ugly, disgusting, amputation ,BadDream, UnrealisticDream*

  2. Details used in the prompt: The model yielded the best results with simple descriptions. The model had some problems with prompts such as "family photo", "man and woman", and the appearance tags usually would mix with eachother. I got around this by testing different appearance tags and switching "and" with "in,with".

  3. Stable Diffusion WebUI with [realistic vision](https://civitai.com/models/4201/realistic-vision-v60-b1), [unrealistic dream](https://civitai.com/models/72437/baddream-unrealisticdream-negative-embeddings) and [lora detail tweaker](https://civitai.com/models/58390/detail-tweaker-lora-lora).[upscaler_4x_NMKD](https://civitai.com/models/141491/4x-nmkd-superscale)

  4. While testing I got better results with **Realistic Vision** rather than [**EpicRealism**](https://civitai.com/models/25694/epicrealism). I followed the recommendations given by  the developer of Realistic Vision. I usually start by creating an image with a low sampling rate (e.g)11 and no upscaling so I can find a adequate seed. After finding a good seed I start using higher sampling rates and tweak the CFG. I got the best results with low CFG 1.5 - 2.5 and unexpectedly it yielded good results with a sampling rate of 6. The biggest change was using the 4x_NMKD-Superscale-SP_178000_G upscaler and lora_detail_tweaker

