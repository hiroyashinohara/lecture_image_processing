# レポート課題２
画像は電機大学のロゴを用いる。

まず初めに以下のコードによって白黒画像に変換した．
ORG = rgb2gray(ORG); colormap(gray); colorbar;
その結果を以下に示す．

![1](https://user-images.githubusercontent.com/19383267/50539638-dbc40e80-0bc6-11e9-88cf-b9dd623e6a0d.PNG)

図１．白黒濃淡画像

次に以下のコードを用いて2諧調画像に変換した．
IMG = ORG>128;
imagesc(IMG); colormap(gray); colorbar;  axis image;

その結果を以下に示す．

![2](https://user-images.githubusercontent.com/19383267/50539639-dbc40e80-0bc6-11e9-98a3-f3fbb4cc5070.PNG)

図２．2諧調画像

同様に、以下の２つコードを用いて4諧調画像および8諧調画像を作成した．
4諧調画像
IMG0 = ORG>64;
IMG1 = ORG>128;
IMG2 = ORG>192;
IMG = IMG0 + IMG1 + IMG2;

8諧調画像
IMG0 = ORG>32;
IMG1 = ORG>64;
IMG2 = ORG>96;
IMG3 = ORG>128;
IMG4 = ORG>160;
IMG5 = ORG>192;
IMG6 = ORG>224;
IMG = IMG0 + IMG1 +IMG2 + IMG3 + IMG4 + IMG5 + IMG6;

その結果をそれぞれ図３．４に示す．

![3](https://user-images.githubusercontent.com/19383267/50539636-db2b7800-0bc6-11e9-97a6-8f38d782a67d.PNG)

図３．4諧調画像

![4](https://user-images.githubusercontent.com/19383267/50539637-dbc40e80-0bc6-11e9-8eab-c4795835f926.PNG)

図４．8諧調画像
