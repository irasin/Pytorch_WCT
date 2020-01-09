# Pytorch_WCT

Unofficial Pytorch(1.0+) implementation of nips paper [Universal Style Transfer via Feature Transforms](https://arxiv.org/pdf/1705.08086.pdf).

Original torch implementation from the author can be found [here](https://github.com/Yijunmaverick/UniversalStyleTransfer).

Other implementations such as [Pytorch_implementation1](https://github.com/black-puppydog/PytorchWCT) , [Pytorch_implementation2](https://github.com/sunshineatnoon/PytorchWCT)  or [Pytorch_implementation3 ](https://github.com/pietrocarbo/deep-transfer)are also available.

This repository provides a pre-trained model for you to generate your own image given content image and style image. 

If you have any question, please feel free to contact me. (Language in English/Japanese/Chinese will be ok!)

## Notice
I propose a structure-emphasized multimodal style transfer(SEMST), feel free to use it [here](https://github.com/irasin/Structure-emphasized-Multimodal-Style-Transfer).

------

## Requirements

- Python 3.7
- PyTorch 1.0+
- TorchVision
- Pillow

Anaconda environment recommended here!

(optional)

- GPU environment 



## Usage

------

## test

1. Clone this repository 

   ```bash
   git clone https://github.com/irasin/Pytorch_WCT
   cd Pytorch_WCT
   ```

2. Prepare your content image and style image. I provide some in the `content` and `style` and you can try to use them easily.

3. Download the pretrained model [here](https://drive.google.com/open?id=1tsaGnC7YbruBQNCp6qMmmaSTJiGuyoPA) and put them under the directory named `model_state`

4. Generate the output image. A transferred output image and a content_output_pair image and a NST_demo_like image will be generated.

   ```python
   python test.py -c content_image_path -s style_image_path
   ```

   ```
   usage: test.py [-h] 
                  [--content CONTENT] 
                  [--style STYLE]
                  [--output_name OUTPUT_NAME] 
                  [--alpha ALPHA] 
                  [--gpu GPU]
                  [--model_state_path MODEL_STATE_PATH]
   
   
   ```

   If output_name is not given, it will use the combination of content image name and style image name.

------

# Result

Some results of content image and my cat (called Sora) will be shown here.

![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/IMG_0565_03_demo.jpg)
![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/IMG_0565_04_demo.jpg)
![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/IMG_0565_05_demo.jpg)
![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/IMG_0565_1_demo.jpg)
![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/IMG_0565_brideg_demo.jpg)
![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/IMG_0565_feathers_demo.jpg)
![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/IMG_0565_horse_demo.jpg)
![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/IMG_0565_hosi_demo.jpg)
![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/IMG_0565_hs6_demo.jpg)
![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/IMG_0565_picasso_seated_nude_hr_demo.jpg.jpg)
![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/IMG_0565_udnie_demo.jpg)
![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/IMG_0565_wave_demo.jpg)


![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/neko_hosi.jpg)



