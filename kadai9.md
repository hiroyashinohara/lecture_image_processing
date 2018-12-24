# レポート課題９
原画像として東京電機大学のロゴを使用した． その画像を以下の図１に示す．
![lenna](https://user-images.githubusercontent.com/19383267/50393837-5262a580-079c-11e9-8fad-1bea341a9679.png)

図１．原画像

課題7と同様に白黒濃淡画像に変換した．
以下の図２に結果を示す．

![1](https://user-images.githubusercontent.com/19383267/50394604-0450a080-07a2-11e9-9b30-601308d28560.PNG)

図２．白黒濃淡画像

以下の手順を用いて白黒濃淡画像にノイズを添付した．
ORG = imnoise(ORG,'salt & pepper',0.02); 
ノイズを添付した画像を以下の図3に示す．

![default](https://user-images.githubusercontent.com/19383267/50395376-e0438e00-07a6-11e9-90d0-e4f12ef2e6b8.PNG)

図３．ノイズ添付結果

ノイズの除去手段として、平滑化フィルタとメディアンフィルタを使用した．

平滑化フィルタの実装手順は以下のとおりである．
IMG = filter2(fspecial('average',3),ORG); 
同様に、メディアンフィルタの実装手順は以下のとおりである．
IMG = medfilt2(ORG,[3 3]);

平滑化フィルタ及びメディアンフィルタでノイズを除去した結果をそれぞれ図４．５に示す．

![2](https://user-images.githubusercontent.com/19383267/50395375-e0438e00-07a6-11e9-9728-ec9aac917961.PNG)

図４．平滑化フィルタによるノイズ除去の結果

![3](https://user-images.githubusercontent.com/19383267/50395378-e0438e00-07a6-11e9-8190-252f0b7da4a2.PNG)

図５．メディアンフィルタによるノイズ除去の結果

以上の結果を見比べると、メディアンフィルタの方が的確にノイズ除去できていることがわかる．

また以下の手段を用いてフィルタを作成、適用した．

f=[0,-1,0;-1,5,-1;0,-1,0]; 
IMG = filter2(f,IMG,'same');

上記の手順によってノイズを除去した結果を以下の図６に示す．

![4](https://user-images.githubusercontent.com/19383267/50395377-e0438e00-07a6-11e9-9cb7-f6a9c49cfc8e.PNG)

図６．作成したフィルタによるノイズ除去

以上より、原画像においてはメディアンフィルタがノイズ除去に適していると考えられる．