# catkin\_make, catkin\_make\_isolated, catkin\_tools\(catkin build\)の違い

**catkin\_make**  
ワークスペース全体をひとつのcmakeプロジェクトとして扱うためビルドが早いが、複数パッケージをビルドする際には依存関係に宣言に注意が必要。一般的なcmakeパッケージはビルドできない。

**catkin\_make\_isolated**  
catkin\_makeの改良版のようなもの。単一のパッケージ毎にビルドしていく。一般的なcmakeパッケージもビルドできる。

**catkin\_tools\(catkin build\)**  
catkin\_make\_isolatedに似ており、単一のパッケージ毎にビルドする。\(一般的なcmakeパッケージもビルドできるか？\)  
catkin\_make\_isolatedに比べ優れている点は、できる場合は複数パッケージを並列ビルドする。  
但し、ここ数年あまり開発されていないらしい。

\[参考\]

[https://answers.ros.org/question/320613/catkin\_make-vs-catkin\_make\_isolated-which-is-preferred/](https://answers.ros.org/question/320613/catkin_make-vs-catkin_make_isolated-which-is-preferred/)

