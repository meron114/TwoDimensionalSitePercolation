# Two-dimensional-site-percolation

　指定した大きさの正方行列で2次元のパーコレーションのシミュレーションができます。

## 説明

　全ての要素が0の正方行列を設定し、そこにランダムに1の要素を上書きしていき、上下もしくは左右の端が1で全て繋がった際に終了します。繋がりの判定は、斜め方向は無しで、縦と横方向のみとしています。A行列は0と1のみの要素で構成されており、C行列は各クラスタが分かるように0とそれ以外の数値の要素で構成されています。C行列の要素の決定は、要素を配置する際に上下左右に隣接する要素を確認し、全て0のみの場合はその時の試行回数の値、0以外の要素が1つある場合はその要素と同じ値、0以外の要素が2つ以上ある場合はその中で一番小さい値を隣接した要素と新しく設定する要素全てに設定しています。尚、最後の要素はマイナス値で設定しています。A行列とC行列および試行回数の結果は、ソースコードで指定した出力先にテキストファイルで出力されます。

[C行列の要素の決定イメージ](images/C.PNG "C")

[100×100行列の結果イメージ](images/100×100.PNG "100×100")

## インストール
　「TwoDimensionsPercolation.exe」をダウンロードし、実行してください

## 使い方
　1. コンソール画面にて正方行列の数値を入力しEnter<br>
　2. 出力ファイルはソースコードに指定された場所を確認

## その他
　ソースコードで実行する場合は[Eigen](https://eigen.tuxfamily.org/index.php?title=Main_Page "Eigen")をインストールして下さい