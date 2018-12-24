# レポート課題１０
原画像として東京電機大学のロゴを使用した．
その画像を以下の図１に示す．

![lenna](https://user-images.githubusercontent.com/19383267/50393837-5262a580-079c-11e9-8fad-1bea341a9679.png)

図１．原画像

課題7と同様に白黒濃淡画像に変換した．
以下の図２に結果を示す．

![1](https://user-images.githubusercontent.com/19383267/50394604-0450a080-07a2-11e9-9b30-601308d28560.PNG)

図２．白黒濃淡画像

エッジの抽出方法として、今回は
プレウィット法
ソベル法
キャニー法
以上の3つの手法を選択した．

MATLABにおけるそれぞれのエッジ抽出の手順は以下のとおりである．
プレウィット法
IMG = edge(ORG,'prewitt');

ソベル法
IMG = edge(ORG,'sobel');

キャニー法
IMG = edge(ORG,'canny');

それぞれのエッジ抽出結果を以下の画像３～５に示す．

![1](https://user-images.githubusercontent.com/19383267/50395691-0bc77800-07a9-11e9-8289-224a27fb2eeb.PNG)

図３．プレウィット法によるエッジ抽出結果

![2](https://user-images.githubusercontent.com/19383267/50395690-0bc77800-07a9-11e9-818f-a13d124bf7d2.PNG)

図４．ソベル法によるエッジ抽出結果

![3](https://user-images.githubusercontent.com/19383267/50395692-0c600e80-07a9-11e9-8f8b-b71259221230.PNG)

図５．キャニー法によるエッジ抽出結果

生成した画像より、キャニー法におけるエッジ抽出は白色が占める割合が比較的多くなるなど、それぞれの方法に特徴がみられた．
