# BLACKDEEP JOB TASK

- Task1 - llm summary
  
  1. Explained in jupyter notebook↑↑↑↑↑
  
- Task2 - Image generation
  1. Prompts Used - **positive prompt** : *a caucasian man in black clothes with brown hair  and a woman with curly black hair and blue eyes,nature,sunset,closeup photo <lora:add_detail:0.5>*,

     **negative prompt** :  *(nsfw, naked, nude, deformed iris, deformed pupils, semi-realistic, cgi, 3d, render, sketch, cartoon, drawing, anime, mutated hands and fingers:1.4), (deformed, distorted, disfigured:1.3), poorly drawn, bad anatomy, wrong anatomy, extra limb, missing limb, floating limbs, disconnected limbs, mutation, mutated, ugly, disgusting, amputation ,BadDream, UnrealisticDream*

  2. Details used in the prompt: I used general appearance prompts such as hair and eyes because it yielded the best results.

  3. Stable Diffusion WebUI with [realistic vision](https://civitai.com/models/4201/realistic-vision-v60-b1), [unrealistic dream](https://civitai.com/models/72437/baddream-unrealisticdream-negative-embeddings) and [lora detail tweaker](https://civitai.com/models/58390/detail-tweaker-lora-lora).

  4. While testing I got better results with **Realistic Vision** rather than [**EpicRealism**](https://civitai.com/models/25694/epicrealism). I followed the recommendations given by  the developer of Realistic Vision and I just tested and tweaked the sampling rate and CFG scale (a lot).

+ Read the README.md in the family photo foldier for generation data
