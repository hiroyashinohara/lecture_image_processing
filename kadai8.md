# レポート課題８
原画像として東京電機大学のロゴを使用した．
その画像を以下の図１に示す．

![lenna](https://user-images.githubusercontent.com/19383267/50393837-5262a580-079c-11e9-8fad-1bea341a9679.png)

図１．原画像

課題7と同様に白黒濃淡画像に変換した．
以下の図２に結果を示す．

![1](https://user-images.githubusercontent.com/19383267/50394604-0450a080-07a2-11e9-9b30-601308d28560.PNG)

図２．白黒濃淡画像

また、図２を閾値128で二値化したものを以下の手順で作成した．
IMG = ORG > 128;
上記によって得られた画像を以下の図３に示す．

![2](https://user-images.githubusercontent.com/19383267/50394603-0450a080-07a2-11e9-8d51-f8db8907fd29.PNG)

図３．二値化後の白黒濃淡画像

また、以下の手順を用いて画像を用いてイメージ内の連結要素をラベル付けした．
IMG = bwlabeln(IMG);
その後以下の手順によってラベル付けされた画像をカラーマップ配列状で表示した．
imagesc(IMG); colormap(jet); colorbar;
その結果を以下の図４に示す．

![default](https://user-images.githubusercontent.com/19383267/50394605-0450a080-07a2-11e9-95dc-1a45ef4da3aa.PNG)

図４．カラーマップ配列画像
