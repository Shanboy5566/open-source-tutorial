# Open source tutorial

這份文件會有兩個部分

1. 安裝Pyhton環境，並使用Python製作Hello World程式

2. 使用人臉情緒辨識套件，進行人臉情緒辨識


## 0. 安裝VSCode

[VSCode](https://code.visualstudio.com/)是一個由微軟開發的程式編輯器，支援多種程式語言，並且有許多套件可以安裝，讓開發更加方便。

安裝完後，打開VSCode

選擇`終端機(Terminal)` > `新增終端機(New terminal)`

## 1-1. 安裝Python環境

檢查系統有無python，有出現版本號代表已安裝

```
python3 --version
```

### For MacOS

```
brew update
brew install python@3.12
```

### For Windows

1. 移至 [開始] 功能表 (左下方的 Windows 圖示)，鍵入 "Microsoft Store"，選取連結以開啟市集。

2. 市集開啟之後，從右上方功能表中選取 [搜尋]，然後輸入 "Python"，選擇3.12的版本。

3. 當 Python 下載結束並完成安裝程序之後，回到VSCode，輸入`python3 --version`，如果有顯示版本號，代表Python已經安裝完成

## 1-2. 安裝Git

檢查系統有無git，有出現版本號代表已安版

```
git --version
```

如果沒有請去[Git官網](https://git-scm.com/downloads)下載安裝


## 1-3. Hello world

請在終端機上執行

```
mkdir -p tutorial
code hello_world.py
```

打開檔案後，輸入以下程式碼

```
print("Hello world")
```

按下`Ctrl + S`儲存檔案

回到終端機，輸入

```
python3 hello_world.py
```

如果有出現`Hello world`，代表程式執行成功

## 2. 使用人臉情緒辨識套件

```
git clone https://github.com/av-savchenko/hsemotion-onnx
```

```
cd hsemotion-onnx
python3 -m venv venv
source venv/bin/activate

python3 -m pip install setuptools mediapipe numpy==1.26.0
python3 setup.py install
python3 demo/recognize_emotions_video.py
```