# レポート課題３
閾値処理を行う．
画像は電機大学のロゴを用いる．

まず初めに以下のコードを用いて白黒濃淡画像を作成する. 
ORG= rgb2gray(ORG); % カラー画像を白黒濃淡画像へ変換
以下の画像１にその結果を示す．

![1](https://user-images.githubusercontent.com/19383267/50539745-b0daba00-0bc8-11e9-9a13-42d530ea8f44.PNG)

図１．白黒濃淡画像

次に、以下のコードを利用して輝度値64を閾値としてその画素を１に、他を０にする．
IMG = ORG > 64;

その結果を以下の図２に示す．

![2](https://user-images.githubusercontent.com/19383267/50539746-b0daba00-0bc8-11e9-8be5-7bbd6a3f615b.PNG)

図２．輝度値64を閾値とした時の2諧調画像

同様に、輝度値が96のとき、128のとき、192のときのコードは以下のとおりである．

IMG = ORG > 96;
IMG = ORG > 128;
IMG = ORG > 192;

それらの結果を以下の図３～５に示す．

![3](https://user-images.githubusercontent.com/19383267/50539741-b0daba00-0bc8-11e9-90c2-21bfa2e1c68e.PNG)

図３．輝度値96

![4](https://user-images.githubusercontent.com/19383267/50539742-b0daba00-0bc8-11e9-8ffd-87bd6e897268.PNG)

図４．輝度値128

![5](https://user-images.githubusercontent.com/19383267/50539743-b0daba00-0bc8-11e9-9bdb-d136aae035a1.PNG)

図５．輝度値192
