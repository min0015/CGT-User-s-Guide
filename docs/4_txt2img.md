# Text to Image

Text to Image(txt2Img, T2I)는 텍스트(텍스트 프롬프트)와 다양한 파라미터, 그리고 ControlNet을 이용해 이미지를 생성하는 Command입니다.

<p><br></p>
![Prompt and Negative Prompt](https://github.com/min0015/CGT-User-s-Guide/blob/main/img/UI_Prompt.png?raw=true)

-   **Prompt**
    -   프롬프트를 입력합니다. <p> 
           
-   **Negative prompt**
    -   네거티브 프롬프트를 입력합니다. 

<p><br></p>
<img width="600" src="/img/UI_Sampler.png?version=4&amp;modificationDate=1718980026249&amp;api=v2" >


-   **Sampler**
    -   샘플러를 선택합니다.
        
        
        -   사용할 수 있는 샘플러  
            Euler / Euler a / LMS / LMS Karras / Heun / DDIM / DDPM / DEIS / LCM / PNDM / UniPC /  
            DPM++ 2M / DPM++ 2M Karras / DPM++ 2M SDE / DPM++ 2M SDE Karras /  
            DPM++ 2S a / DPM++ 2S a Karras / DPM++ SDE / DPM++ SDE Karras /  
            DPM2 / DPM2 Karras / DPM2 a / DPM2 a Karras  <p>
              
            
-   **Sampling Steps**
    -   샘플러가 적용되는 스텝 수를 입력합니다. (최소 1, 최대 100)  <p>
    
<p><br></p>
<img width="600" src="/img/UI_W_H_CFG.png?version=2&amp;modificationDate=1718979766731&amp;api=v2" >

-   **Width**
    -   생성할 이미지의 가로 크기(pixel)를 입력합니다. (최소 8, 최대 2048) <p>
-   **Height**
    -   생성할 이미지의 세로 크기(pixel)를 입력합니다. (최소 8, 최대 2048) <p>
-   **CFG Scale**
    -   CFG Scale을 입력합니다. (최소 1, 최대 20) <p>

<p><br></p>
<img width="600" src="/img/UI_Seed_LoRA.png?version=2&amp;modificationDate=1718980283184&amp;api=v2" >

-   **Seed**
    -   Seed 값을 입력합니다.
        -   -1 : 랜덤 값이 적용됩니다. 적용된 Seed 값은 생성 후 Recipe Result Metadatas 칸에 표시됩니다.
        -   큐브 아이콘 버튼 : -1 값이 입력됩니다.
        -   리싸이클 아이콘 버튼 : 바로 전 생성에 적용되었던 Seed 값이 입력됩니다. <p>  
              
            
-   **LoRA Model**
    -   사용할 LoRA 모델의 파일이름을 입력합니다. Models Tab에서 LoRA 파일을 선택하고 Add 버튼을 눌러 입력할 수도 있습니다.   <p>
          
        
-   **Delete**
    -   입력한 LoRA 모델을 삭제(선택 해제)합니다.   <p>
          
        
-   **LoRA Scale**
    -   사용할 LoRA 파일의 적용 값을 입력합니다. (최소 0, 최대 2)   <p>

<p><br></p>
<img width="600" src="/img/UI_CN_Image.png?version=1&amp;modificationDate=1718979888722&amp;api=v2" >

-   **ControlNet Tab**
    -   이미지 생성에 ControlNet을 사용합니다. 최대 5개까지 ControlNet을 사용할 수 있습니다.  
          
        
-   **Upload (Image)**
    -   ControlNet에 사용할 소스 이미지를 업로드 합니다. 이 칸을 클릭 하여 브라우저를 열거나 이미지 파일을 직접 드래그&드랍 으로 옮겨넣을 수 있습니다.  
        
-   **Preview (Image)**
    -   Preprocessor를 선택하고 Preview 버튼을 누르면 전처리 기능을 거쳐 소스 이미지가 표시됩니다. (현재 사용할 수 없습니다.)  

<p><br></p>
<img width="600" src="/img/UI_CN_enable.png?version=1&amp;modificationDate=1718979926314&amp;api=v2" >

-   **enable**
    -   해당 Tab의 ControlNet 기능이 동작되도록 합니다.  
          
        
-   **Preprocessor**
    -   ControlNet의 전처리 기능을 선택합니다. (현재 사용할 수 없습니다.)  
          
        
-   **Model**
    -   사용할 ControlNet 모델을 선택합니다.
        
        -   사용할 수 있는 ControlNet 모델  
            Canny / Depth / Tile / Openpose / Inpaint  
              
            
-   **Weight**
    -   사용할 ControlNet의 강도를 입력합니다. (최소 0, 최대 1)  

<p><br></p>
<img width="600" src="/img/UI_CN_ColorFix.png?version=1&amp;modificationDate=1718979957975&amp;api=v2" >

-   **Color Fix**
    -   ControlNet 모델 중 Tile을 사용할 경우, 색 보정을 실행합니다.  
          
        
-   **Sharpen**
    -   ControlNet 모델 중 Tile을 사용할 경우, 색 보정과 함께 적용되는 Sharpen 효과값을 입력합니다. (최소 0, 최대 2)  
          
        
-   **Blur Radius**
    -   ControlNet 모델 중 Tile을 사용할 경우, 색 보정과 함께 적용되는 Blur 효과값을 입력합니다. (최소 1, 최대 32)  
          
        
-   **Preview**
    -   ControlNet의 전처리 기능을 실행하여 Preview 칸에 표시합니다. (현재 사용할 수 없습니다.)
