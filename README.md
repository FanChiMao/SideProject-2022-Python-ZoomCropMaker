# SideProject-2022-Python-ZoomCropMaker

## 1. Preparation 
Place the images you want to process in [./imgs](imgs).  

## 2. Run
After placing the images, check the [**config.yaml**]().
```
###############
IMG:
  TYPE: 'png'  # 'jpg' , '' , ...

PATH:
  INPUT_DIR: './imgs'
  SAVE_DIR: './results'

CROP:
  NUMBER: 2       # total cropping patch number
  RANDOM: False    # True, False: crop the patches by random select
  POSITION: 'R'   # 'L'(eft), 'R'(ight), 'T'(op), 'B'(ottom)
  BOX_SIZES: 50   # the size of boundary box (pixel * pixel)
  BOX_THICK: 1    # thickness of boundary box (pixel)
  BOX_LOCAT: [[100, 100], [250, 250]]        # the pixel location of top-left corner [y, x]
  BOX_COLOR: [[0, 0, 255], [0, 255, 0]]  # the color of boundary box [B, G, R]

```

Then, simply run the code `zoom_and_combine.py` or typing the code in terminal. 
```
python zoom_and_combine.py
```

## 3. Final examples  
- Example result 1:

    <details>  
    <summary><strong>config.yaml</strong></summary>  
  
    ```
      ###############
      IMG:
        TYPE: 'png'  # 'jpg' , '' , ...
    
      PATH:
        INPUT_DIR: './imgs'
        SAVE_DIR: './results'
    
      CROP:
        NUMBER: 2       # total cropping patch number
        RANDOM: False    # True, False: crop the patches by random select
        POSITION: 'R'   # 'L'(eft), 'R'(ight), 'T'(op), 'B'(ottom)
        BOX_SIZES: 50   # the size of boundary box (pixel * pixel)
        BOX_THICK: 1    # thickness of boundary box (pixel)
        BOX_LOCAT: [[100, 100], [250, 250]]        # the pixel location of top-left corner [y, x]
        BOX_COLOR: [[0, 0, 255], [0, 255, 0]]  # the color of boundary box [B, G, R]
    
    ```
    </details>  

    <img src="https://i.imgur.com/2n5yXgl.png" alt="noise2" width="800" style="zoom:100%;" />
    
- Example result 2:

    <details>  
    <summary><strong>config.yaml</strong></summary>  
  
    ```
      ###############
      IMG:
        TYPE: 'png'  # 'jpg' , '' , ...
    
      PATH:
        INPUT_DIR: './imgs'
        SAVE_DIR: './results'
    
      CROP:
        NUMBER: 3       # total cropping patch number
        RANDOM: False    # True, False: crop the patches by random select
        POSITION: 'B'   # 'L'(eft), 'R'(ight), 'T'(op), 'B'(ottom)
        BOX_SIZES: 50   # the size of boundary box (pixel * pixel)
        BOX_THICK: 1    # thickness of boundary box (pixel)
        BOX_LOCAT: [[100, 100], [250, 250], [400, 89]]      # the pixel location of top-left corner [y, x]
        BOX_COLOR: [[0, 0, 255], [0, 255, 0], [255, 0, 0]]  # the color of boundary box [B, G, R]
    
    ```
    </details>  

    <img src="https://i.imgur.com/RpDMSby.png" alt="noise2" width="600" style="zoom:100%;" />


- Example result 3:

    <details>  
    <summary><strong>config.yaml</strong></summary>  
  
    ```
      ###############
      IMG:
        TYPE: 'png'  # 'jpg' , '' , ...
      
      PATH:
        INPUT_DIR: './imgs'
        SAVE_DIR: './results'
      
      CROP:
        NUMBER: 4       # total cropping patch number
        RANDOM: True    # True, False: crop the patches by random select
        POSITION: 'L'   # 'L'(eft), 'R'(ight), 'T'(op), 'B'(ottom)
        BOX_SIZES: 75   # the size of boundary box (pixel * pixel)
        BOX_THICK: 2    # thickness of boundary box (pixel)
        BOX_LOCAT: [[100, 100], [250, 250]]        # the pixel location of top-left corner [y, x]
        BOX_COLOR: [[0, 0, 255], [0, 255, 0]]  # the color of boundary box [B, G, R]
          
    ```
    </details>  

    <img src="https://i.imgur.com/GIE5mkr.png" width="800" style="zoom:100%;" />

- Example result 4:

    <details>  
    <summary><strong>config.yaml</strong></summary>  
  
    ```
      ###############
      IMG:
        TYPE: 'png'  # 'jpg' , '' , ...
      
      PATH:
        INPUT_DIR: './imgs'
        SAVE_DIR: './results'
      
      CROP:
        NUMBER: 5       # total cropping patch number
        RANDOM: True    # True, False: crop the patches by random select
        POSITION: 'T'   # 'L'(eft), 'R'(ight), 'T'(op), 'B'(ottom)
        BOX_SIZES: 40   # the size of boundary box (pixel * pixel)
        BOX_THICK: 3    # thickness of boundary box (pixel)
        BOX_LOCAT: [[100, 100], [250, 250]]        # the pixel location of top-left corner [y, x]
        BOX_COLOR: [[0, 0, 255], [0, 255, 0]]  # the color of boundary box [B, G, R]

    ```
    </details>  

    <img src="https://i.imgur.com/Oj5pzml.png" width="600" style="zoom:100%;" />

## 4. Contact  
If you have any question or suggestion, feel free to contact us:  
- [**Chi-Mao Fan**](https://github.com/FanChiMao): qaz5517359@gmail.com  
- [**X-X X**](https://github.com/bobo0303): wiwi61666166@gmail.com  
