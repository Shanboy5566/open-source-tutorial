# Open source tutorial

這份文件會有兩個部分

1. 安裝Pyhton環境，並使用Python製作Hello World程式

2. 使用人臉情緒辨識套件，進行人臉情緒辨識


## 0. 打開終端機

### For MacOS

按下`Command + Space`，輸入`Terminal`，按下`Enter`即可打開終端機

### For Windows

按下`Win + R`，輸入`cmd`，按下`Enter`即可打開終端機

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
git clone https://github.com/Shanboy5566/open-source-tutorial.git
```

接著進入資料夾

```
cd open-source-tutorial
```

執行`hello.py`

```
python3 hello_world.py
```

如果有出現`Hello world`，代表程式執行成功

## 2. 使用人臉情緒辨識套件

```
python3 -m venv venv
source venv/bin/activate

pyton3 -m pip install --upgrade pip
python3 -m pip install -r requirements.txt
python3 recognize_emotions_video.py
```
