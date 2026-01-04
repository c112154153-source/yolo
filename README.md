# Aortic Valve Detection with YOLOv12 (期末專題報告程式碼)

本專案為機器學習期末報告之原始程式碼，使用 YOLOv12 模型進行主動脈瓣 (Aortic Valve) 的偵測。本文件說明如何配置環境、執行訓練與預測，以協助第三方使用者重現競賽結果。

## 1. 安裝配置環境 (Installation & Environment)

本專案建議於 **Google Colab** 或具備 NVIDIA GPU 的 Linux/Windows 環境下執行。

### 核心依賴套件
* **Python**: 3.8+
* **PyTorch**: 建議搭配 CUDA 12.1 以支援 GPU 加速
* **Ultralytics**: 用於 YOLO 模型訓練與推論

### 安裝指令
請依序執行以下指令以安裝所需套件：
```bash
# 安裝 PyTorch (請依據您的 CUDA 版本調整 index-url)
pip install torch torchvision torchaudio --index-url [https://download.pytorch.org/whl/cu121](https://download.pytorch.org/whl/cu121)

# 安裝 YOLO 核心庫
pip install ultralytics
