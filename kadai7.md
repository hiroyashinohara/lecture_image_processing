# レポート課題７
原画像として東京電機大学のロゴを使用する．
以下の図１に原画像を示す．

![lenna](https://user-images.githubusercontent.com/19383267/50393837-5262a580-079c-11e9-8fad-1bea341a9679.png)

図１．原画像

rgb2grayを用いて、白黒濃淡画像に変化させた．その結果を以下の図２に示す．

![1](https://user-images.githubusercontent.com/19383267/50394193-50e6ac80-079f-11e9-88ac-83ee6ee97301.PNG)

図２．白黒濃淡画像

その時の濃度ヒストグラムを作成した．以下の図３に示す．

![2](https://user-images.githubusercontent.com/19383267/50394192-50e6ac80-079f-11e9-8f9d-8a74d5f98fe8.PNG)

図３．濃度ヒストグラム

また、原画像のダイナミックレンジを0から255に変更した．その時の画像を以下の図４に示す．

![3](https://user-images.githubusercontent.com/19383267/50394196-50e6ac80-079f-11e9-95c3-155029ed94ad.PNG)

図４．ダイナミックレンジ変更後

ORG=unit8(ORG)によって、画像を8ビット符号なし整数配列に変更した．
その状態で濃度ヒストグラムを生成した．以下の図５に濃度ヒストグラムを示す．

![4](https://user-images.githubusercontent.com/19383267/50394194-50e6ac80-079f-11e9-89a5-5ba8786a37e5.PNG)

図５．濃度ヒストグラム
