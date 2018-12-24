# 課題１レポート

今回は原画像として、東京電機大学のロゴを使用した．

現画像を1/2サンプリングせずに表示した結果を図１に示す．

![lenna](https://user-images.githubusercontent.com/19383267/50393347-03ffd780-0799-11e9-9c54-85b4bad38bed.png)

図1 原画像

1/2サンプリングの結果を図２に示す．


![1](https://user-images.githubusercontent.com/19383267/50393400-61942400-0799-11e9-9d10-6183ef359474.PNG)

図2 1/2サンプリング

同様に原画像をさらに1/2サンプリングしていくには

IMG = imresize(ORG,0.5); % 画像の縮小  
IMG2 = imresize(IMG,2,'box'); % 画像の拡大

とすればよい．1/4サンプリングから1/64サンプリングの結果を以下の図3～6に示す．

![2](https://user-images.githubusercontent.com/19383267/50393408-7375c700-0799-11e9-8632-f7c7d9c27bf4.PNG)

図3 1/4サンプリング

![3](https://user-images.githubusercontent.com/19383267/50393416-87212d80-0799-11e9-81b6-3b6f76f6d9fc.PNG)

図4 1/8サンプリング

![4](https://user-images.githubusercontent.com/19383267/50393415-86889700-0799-11e9-97ed-fe321414b330.PNG)

図5 1/16サンプリング

![5](https://user-images.githubusercontent.com/19383267/50393418-87212d80-0799-11e9-8ecb-319bae2cc236.PNG)

図6 1/32サンプリング

![6](https://user-images.githubusercontent.com/19383267/50393417-87212d80-0799-11e9-92d0-948f92e86485.PNG)

図7 1/64サンプリング


サンプリングの幅が大きくなるにつれて、モザイクの大きさも同様に大きくなっていることがわかる．
