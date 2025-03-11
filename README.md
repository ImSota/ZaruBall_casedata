# ZaruBall用3Dプリントデータ
ZaruBallは現状サンドイッチマウントのみに対応しています。<br>
~~2ピースケース、25mmボール用トラックボールケースを今後設計予定です。~~<br>
2025/3/11 2ピースケースのデータを公開しました。

## 2ピースケース
2ピースケースは需要を鑑み、親指クラスタがchoc v2スイッチに対応したものを公開しています。<br>
![2P_case](/image/2Pcase.png)
3Dプリントするデータは以下の通りです。
| 左右 | データ名 | 説明  |
| ---- | ---- | ---- |
| 左 | L_top.stl | 左手のトップケース |
| 左 | L_bottom.stl | 左手のボトムケース |
| 左 | knob.stl | ロータリーエンコーダにつけるノブ |
| 右 | R_top.stl | 右手のトップケース |
| 右 | R_bottom.stl | 右手のボトムケース |
| 右 | 34mm_trackball_case_for2P.stl | マグネット固定対応34mmボールケース |
| 両方 | power_switch.stl | 電源スイッチカバー |
| 両方 | reset_switch.stl | リセットスイッチ押下用ピン |

3Dプリントパーツの他にも用意するパーツがあります。
| 用意するパーツ | 点数 | 寸法 |
| ---- | ---- | ---- |
| ネオジム磁石 | 30個 | 直径2mm, 高さ2mmの円筒形 |
| セラミックボール | 2個 |  直径2mm |
| ゴム足 | 8個 | 直径10mm |

### 組み立て方法
右手側のケース組み立て手順をご説明します。左手側もほぼ同様の手順で組み立てられます。
1. マグネットをトップケース、ボトムケース、トラックボールケースに圧入します。マグネットが入らない場合は2mmのドリルやマイナスドライバで穴を拡張します。緩く、マグネットが抜けてしまう場合は接着剤を穴に少量入れて固定してください。
    ![insert magnet](/image/magnet.jpg)
2. セラミックボール3つをトラックボールケースに圧入します。固いものを押し当てることで簡単に圧入することができます。
    ![insert_ceramic ball](/image/ceramicball.jpg)
3. トップケースにリセットスイッチピンを入れます
    ![insert reset switch pin](/image/insert_resetswitch.jpg)
4. PCBをトップケースにはめ込む。この時USB端子と電源スイッチをケースの穴にはめ込むようにします。また、リセットスイッチピンが抜けないよう逆さにしたまま作業します。
    ![insert PCB](/image/insert_pcb.jpg)
5. 四隅にスイッチをはめて、PCBとトップケースを固定します
    ![insert switches](/image/insert_switch.jpg)
6. ゴム足を貼ります。ボトムケースにはゴム足固定用のくぼみがあるのでそこに合わせて貼り付けてください。
    ![putting rubberfeet](/image/rubberfeet.jpg)
7. バッテリをボトムケースにマスキングテープ等で固定します。厚みがある方に寄せて配置してください。
    ![pinning battery](/image/battery.jpg)
8. バッテリコネクタを接続し、ボトムケースとトップケースをマグネットで固定します。
9. 電源スイッチカバーを取り付けます。
    ![putting power switch cover](/image/power_switch_cover.jpg)
10. トラックボール基板のマグネットコネクタをPCBと接続し、トラックボール基板の上からトラックボールケースをかぶせます。
    ![trackball connect](/image/trackball.jpg)
11. すべてのスイッチとキーキャップ、トラックボールを取り付けます。
12. マイコンのインジケータLEDの確認穴に2mmのアクリル丸棒を差し込むことで光が拡散し見やすくなります。
    ![insert acrylic rod](/image/acrylic_rod.jpg)


## サンドイッチマウントケース
ZaruBallは親指クラスタのみMXスイッチとChoc v2スイッチに対応、その他はMXスイッチの実に対応しています。親指クラスタにMXスイッチを用いる場合とChocスイッチを利用する場合で使用するプレートデータが異なります。<br>

### サンドイッチマウントで共通する注意事項
- トッププレートはマイコン部分のでっぱりを収めるように該当部分を少し薄くしてあります。
そのため、キーキャップが乗る面がビルドプレートに面するように向きを変更してください。
- プリントするパーツ以外にm2ねじ24本と7mmスペーサ12個が必要です。

### 親指クラスタにMXスイッチを使用するケース
データ保管先：
[case/mx_thumb_sandwichcase](case/mx_thumb_sandwichcase)<br>

プリントする3Dモデル：
- right_topplate.obj (右手用トッププレート)
- right_bottomplate.obj (右手用ボトムプレート)
- left_topplate.obj (左手用トッププレート)
- left_bottomplate.obj (左手用ボトムプレート)

### 親指クラスタにChoc v2スイッチを使用するケース
![chocv2_thumb_case](/image/chocthumb.png)
データ保管先：
[chocv2_thumb_sandwichcase](chocv2_thumb_sandwichcase)<br>

プリントする3Dモデル：
- right_choc_plate.obj (右手Chocスイッチ用トッププレート)
- right_mx_plate.obj (右手MXスイッチ用トップ    プレート)
- right_bottom_plate.obj (右手用ボトムプレート)
- left_choc_plate.obj (左手Chocスイッチ用トッププレート)
- left_mx_plate.obj (左手MXスイッチ用トッププレート)
- left_bottom_plate.obj (左手用ボトムプレート)


## 34mm トラックボールケース
- 34mm_trachball_case.obj 

ZaruBallでは独自のトラックボール基板を採用しています。keyballやroBa, moNaのトラックボールケースは使用できません。<br>
トラックボールケースに2mmのセラミックボールを挿入してください。ドライバ―の裏側などで強く押し込むことで圧入できます。<br>

トラックボールケースはKeyball Trackball Case (Test)（https://www.thingiverse.com/thing:6749719
）を改変して公開しています。<br>
© kepeo (クリエイティブ・コモンズ・ライセンス（表示4.0 国際）https://creativecommons.org/licenses/by/4.0/
