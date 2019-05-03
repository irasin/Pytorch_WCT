# Pytorch_WCT

Unofficial Pytorch(1.0+) implementation of nips paper [Universal Style Transfer via Feature Transforms](https://arxiv.org/pdf/1705.08086.pdf).

Original torch implementation from the author can be found [here](https://github.com/Yijunmaverick/UniversalStyleTransfer).

Other implementations such as [Pytorch_implementation1](https://github.com/black-puppydog/PytorchWCT) , [Pytorch_implementation2](https://github.com/sunshineatnoon/PytorchWCT)  or [Pytorch_implementation3 ](https://github.com/pietrocarbo/deep-transfer)are also available.

This repository provides a pre-trained model for you to generate your own image given content image and style image. 

If you have any question, please feel free to contact me. (Language in English/Japanese/Chinese will be ok!)

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
   python test -c content_image_path -s style_image_path
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

![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/res1.gif)
![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/res3.gif)
![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/res4.gif)
![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/res5.gif)
![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/neko_hosi.jpg)
![image](https://github.com/irasin/Pytorch_WCT/blob/master/res/neko_hosi_style_transfer_demo.jpg)



