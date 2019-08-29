# 恒星の座標データから星座を描画する  


## 開発環境  

- Windows10(64bit)  
- Python 3.7.3  
    - matplotlib 3.1.1  
    - numpy 1.17.0  
- EmEditor  

## 準備  

- Python仮想環境を作る
```
C:\>
C:\>python3 -m virtualenv seiza
C:\>cd seiza
C:\seiza>Scripts\activate.bat
(seiza) C:\seiza>
(seiza) C:\seiza>
```

- pipを使ってライブラリをインストールする  

```
pip install numpy
pip install matplotlib
```

## アプリ  

### make-seiza.py  

恒星の座標データは [HYG 3.0](http://www.astronexus.com/files/downloads/hygdata_v3.csv.gz) を使用。  

- 機能
    - 恒星の座標データを基に星座を描く
    - 指定した星座の画像をPDF形式とPNG形式に出力する

```
使い方

> python3 make-seiza.py 星座名(略称) 視等級 出力ファイル形式

```

```
使用例：オリオン座で4等級以上の恒星をPNG形式で出力する

> python3 make-seiza-sqlite.py Ori 4 png

```

 
