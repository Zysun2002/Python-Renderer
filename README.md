# Alberta-Renderer
This project is part of my 3-month research internship program in the University of Alberta. 


## Introduction

This renderer is for learning purpose. You could learn how to implement a python renderer from scratch from this project.

The renderer is a expended python version of [Dmitry V. Sokolov](https://github.com/ssloy/tinyrenderer)'s tutorial on computer graphics and rendering. Besides including all the features introduced in his tutorial, the advance made in this version is:
1. This renderer is implemented in Python. This is because I hope to integrate it with some other rendering techniques (like neural rendering) in the future.
2. This renderer supports to render a scene with multiple objects. 
3. This renderer supports obj and mtl file format. This is because I found obj + mtl can be easily found on the internet and thus the renderer can render more 3D assets.

Though implemented using python, the renderer does not rely on high-level graphics library during rendering process. I gain fundamental knowledge about rendering and computer graphics during building my renderer step by step.

## Selected Features：

### ambient and specular light
I really love the ambient and specular light which make the material look like more real. By calculating the angle between the reflection and the eye direction, the specular highlight is rendered.

you can render your 3D assets using these 
```
cd mtl_parse
python main.py --ratio_Ka YOUR_RATIO_KA --ratio_KD YOUR_RATIO_KD --ratio_Ks YOUR_RATIO_KS
```

### Shadow mapping technique
An easy way to make rendering more photo-realistic is to calculate more accurate shadow. By a two-pass rendering process, we could bake the shadow information in a shadow mapping previously before real rendering.





### Appendix
 The project is still ongoing.


![poster pre](https://github.com/user-attachments/assets/ff284f99-b100-4782-b07e-e0cec28ad572)
A presentation in the poster fair organized by UofA. **You can review my poster [here](https://github.com/Zysun2002/Renderer-Alberta/blob/main/poster_ZiyuSun.pdf).**

![weareworldshapers](https://github.com/user-attachments/assets/39145eb4-3d7e-4bbd-b364-68452094053f)
The sentence that inspired me most.
