# helmet_detection
Use YOLOv8 to train an object detection model to detect cyclists, license plates, helmeted riders, and non-helmeted riders on the road.

# Python版本 3.8 torch 2.4.0+cu118 

資料讀取與統計:
讀取所有標籤文件，統計每種標籤的數量。  
![示例截圖01](https://github.com/wenshenfan/helmet_detection/raw/main/screenshot/01.jpg)


影像繪製:
在影像上繪製邊框和標籤。  
![示例截圖01](https://github.com/wenshenfan/helmet_detection/raw/main/screenshot/02.jpg)


創建訓練配置文件"data.yaml"，保存模型權重。  
![示例截圖03](https://github.com/wenshenfan/helmet_detection/raw/main/screenshot/03.jpg)


使用yolov8官網提供的yolov8n.pt作為預訓練模型。  
![示例截圖04](https://github.com/wenshenfan/helmet_detection/raw/main/screenshot/04.jpg)


設定模型訓練參數，開始訓練。  
![示例截圖05_1](https://github.com/wenshenfan/helmet_detection/raw/main/screenshot/05_1.jpg)
![示例截圖05_2](https://github.com/wenshenfan/helmet_detection/raw/main/screenshot/05_2.jpg)
![示例截圖05_3](https://github.com/wenshenfan/helmet_detection/raw/main/screenshot/05_3.jpg)


將訓練完的模型best.pt複製到models目錄  
![示例截圖06](https://github.com/wenshenfan/helmet_detection/raw/main/screenshot/06.jpg)


使用訓練完的模型做圖片的物件偵測。  
![示例截圖07_1](https://github.com/wenshenfan/helmet_detection/raw/main/screenshot/07_1.jpg)
![示例截圖07_2](https://github.com/wenshenfan/helmet_detection/raw/main/screenshot/07_2.jpg)

使用訓練完的模型做影片的物件偵測，將影片放入input目錄中，並改名為input_video.mp4，執行程式後在output資料夾匯出物件偵測影片結果。  
![示例截圖08_1](https://github.com/wenshenfan/helmet_detection/raw/main/screenshot/08_1.jpg)
![示例截圖08_2](https://github.com/wenshenfan/helmet_detection/raw/main/screenshot/08_2.jpg)
![示例截圖08_3](https://github.com/wenshenfan/helmet_detection/raw/main/screenshot/08_3.jpg)
![示例截圖08_4](https://github.com/wenshenfan/helmet_detection/raw/main/screenshot/08_4.jpg)
