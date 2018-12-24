# 課題１レポート

今回は原画像として、東京電機大学のロゴを使用した．

現画像を1/2サンプリングせずに表示した結果を図１に示す．

![lenna](https://user-images.githubusercontent.com/19383267/50393347-03ffd780-0799-11e9-9c54-85b4bad38bed.png)
図1 原画像

1/2サンプリングの結果を図２に示す．

![原画像](https://github.com/mackhasegawa/lecture_image_processing/blob/master/image/kadai1_1.png?raw=true)  
図2 1/2サンプリング

同様に原画像をさらに1/2サンプリングしていくには

IMG = imresize(ORG,0.5); % 画像の縮小  
IMG2 = imresize(IMG,2,'box'); % 画像の拡大

とすればよい．1/4サンプリングから1/32サンプリングの結果を以下の図3～6に示す．

![原画像](https://github.com/mackhasegawa/lecture_image_processing/blob/master/image/kadai1_2.png?raw=true)  
図3 1/4サンプリング

![原画像](https://github.com/mackhasegawa/lecture_image_processing/blob/master/image/kadai1_3.png?raw=true)  
図4 1/8サンプリング

![原画像](https://github.com/mackhasegawa/lecture_image_processing/blob/master/image/kadai1_4.png?raw=true)  
図5 1/16サンプリング

![原画像](https://github.com/mackhasegawa/lecture_image_processing/blob/master/image/kadai1_5.png?raw=true)  
図6 1/32サンプリング

サンプリングの幅が大きくなるにつれて、モザイクの大きさも同様に大きくなっていることがわかる．
