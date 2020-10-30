# sigverse_urm_dataset

## はじめに
このデータセットは、SIGVerseを使って収集した被験者の頭、胴体、左手、右手の時系列データをまとめたものです。  

RoboCup@Home SimulationのHuman Navigationタスクの環境を用いて、被験者10人に対してそれぞれ25セッション取り組んでもらい、その時の動作データを時系列に収集しました。  
その後、 第三者が被験者の動作を見ながら「悩んでいる」「悩んでいない」のラベル付けしました。  



## データの見方
csvファイルには以下のような並びでデータが入っています。（データは20Hzの周期で収集しました）

| ElapsedTime | Body | Head | LeftHand | RightHand | SubjectiveLabel |
| :---: | :---: | :---: | :---: | :---: | :---: |
| time_stamp  | x, y, z, qx, qy, qz, w | x, y, z, qx, qy, qz, w | x, y, z, qx, qy, qz, w | x, y, z, qx, qy, qz, w | 0(Avatar understands) / 1(Avadar doesn't understand) / 2(Indistinguishable)|
| 0.00  | x, y, z, qx, qy, qz, w | x, y, z, qx, qy, qz, w | x, y, z, qx, qy, qz, w | x, y, z, qx, qy, qz, w | 0 |
| 0.05  | x, y, z, qx, qy, qz, w | x, y, z, qx, qy, qz, w | x, y, z, qx, qy, qz, w | x, y, z, qx, qy, qz, w | 0 |
| ... | ... | ... | ... | ... | ... |




## 注意事項
- データ収集時の不手際で、被験者01の第13セッションと、被験者09の第15セッションが抜けています。
