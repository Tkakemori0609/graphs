import matplotlib.pyplot as plt
# データ準備
numbers_list = list(map(int, input("数値を入力してください").split()))
values_list = list(map(str,input("数値と同じだけの数の名前を入力してください").split()))
# The pyplot APIでの描画
plt.figure(figsize=(9, 3)) # 描画するサイズを決める
plt.subplot(131) # 1行3列の左から1番目をこれから操作しますよ
plt.bar(values_list,numbers_list) # 棒グラフ
plt.subplot(132) # 1行3列の左から2番目をこれから操作しますよ
plt.scatter(values_list,numbers_list) # 散布図
plt.subplot(133) # 1行3列の左から3番目をこれから操作しますよ
plt.plot(values_list,numbers_list) # 折れ線グラフ

plt.suptitle("Graphs") # タイトルの設定
plt.show() # 描画
