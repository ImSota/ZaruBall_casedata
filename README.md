# ZaruBall用3Dプリントデータ
ZaruBallのケース、トラックボールケース、ロータリーエンコーダー用ノブのstlファイルを公開しています。<br>
ケースは需要を鑑み、親指クラスタがchoc v2スイッチに対応したものを公開しています。<br>
全てMXスイッチのZaruBallを作成したい方は簡易的なサンドイッチプレートマウントのケースを使用してください。

トラックボールケースはKeyball Trackball Case (Test)（https://www.thingiverse.com/thing:6749719
）を改変して公開しています。<br>
© kepeo (クリエイティブ・コモンズ・ライセンス（表示4.0 国際）https://creativecommons.org/licenses/by/4.0/

![2P_case](/image/2Pcase.png)

## ケース
データ画保管先は[こちら](/case/normal_case)<br>
3Dプリントするデータは以下の通りです。
| 左右 | データ名 | 説明  |
| ---- | ---- | ---- |
| 左 | L_top.stl | 左手のトップケース |
| 左 | L_bottom.stl | 左手のボトムケース |
| 左 | knob.stl | ロータリーエンコーダにつけるノブ |
| 右 | R_top.stl | 右手のトップケース |
| 右 | R_bottom.stl | 右手のボトムケース |
| 右 | 34mm_trackball_case.stl | マグネット固定対応34mmボールケース |
| 右 | 25mm_trackball_case.stl | マグネット固定対応25mmボールケース |
| 両方 | power_switch.stl | 電源スイッチカバー |
| 両方 | reset_switch.stl | リセットスイッチ押下用ピン |

トラックボールケースはお好みのサイズを選択してください。

3Dプリントパーツの他にも用意するパーツがあります。
| 用意するパーツ | 点数 | 寸法 |
| ---- | ---- | ---- |
| ネオジム磁石 | 30個 | 直径2mm, 高さ2mmの円筒形 |
| セラミックボール | 3個 |  直径2mm |
| ゴム足 | 8個 | 直径10mm |

### 印刷時の設定・注意点
<details>
    <summary>詳細</summary>

印刷はすべてCreality社製K1CとK1Maxを用いて0.4mmノズルの0.2mm積層でテストしております。
異なる環境では下記の設定ではうまくプリントできない可能性があります。

#### トップケース
自動サポートを使用するとUSBコネクタ回りのサポートが歯がしにくく、ハマりにくくなるので非推奨です。
サポートを配置するのはマイコンカバーとトラボ基板と接続するマグネットコネクタ回りの2点のみです。
ツリー形状のサポートがいいかと思います。マグネットコネクタ周りのサポートはブリッジの中央付近に小さめのサポートを配置するだけで大丈夫です。<br>
画像はサポート設定の例です。緑色の部分がサポートとなる箇所です。
![topcase setting](/image/top_setting.png "緑色の部分がサポートとなる箇所です。")

#### ボトムケース
ボトムケースはサポートなしで印刷可能です。stlファイルをスライサにインポートした状態では傾いた状態となっているので、底面がビルドプレートに触れるように配置してください。
![bottomcase setting](/image/bottom_setting.png "底面をビルドプレートに設置")

#### リセットスイッチピン / 電源スイッチカバー / ノブ
リセットスイッチピン、電源スイッチカバー、ノブは以下の画像のような向きにしてプリントしてください。
リセットスイッチピンはブリムをつけておくとビルドプレートから外れにくくなります。
![reset, power switch setting](/image/reset_powerswitch_setting.png)

#### 34mmトラックボールケース
手動サポートにてマグネットコネクタ用の開口部のみにサポートを配置します。
トラックボール基板が収納されるケース部分にサポートを配置すると除去が困難になるので注意しましょう。
![trackball case setting](/image/trackball_setting.png)

            
#### 25mmトラックボールケース
動作未確認のため、後ほど追記します。
</details>

### 組み立て方法
<details>
    <summary>詳細</summary>

右手側のケース組み立て手順をご説明します。左手側もほぼ同様の手順で組み立てられます。
1. マグネットをトップケース、ボトムケース、トラックボールケースに圧入します。マグネットが入らない場合は2mmのドリルやマイナスドライバで穴を拡張します。緩く、マグネットが抜けてしまう場合は接着剤を穴に少量入れて固定してください。<br>
ボトムケースのトラックボール固定用マグネットは25mmボールと35mmボールで配置が異なります。トラックボールケースをボトムケースに当てはめてみて適切なマグネットの位置を探してください。
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
11. すべてのスイッチとキーキャップ、トラックボール、ノブを取り付けます。
12. マイコンのインジケータLEDの確認穴に2mmのアクリル丸棒を差し込むことで光が拡散し見やすくなります。
    ![insert acrylic rod](/image/acrylic_rod.jpg)
</details>

## サンドイッチマウントケース

ZaruBallは親指クラスタのみMXスイッチとChoc v2スイッチに対応、その他はMXスイッチのみに対応しています。親指クラスタにMXスイッチを用いる場合とChocスイッチを利用する場合で使用するプレートデータが異なります。<br>

<details>
    <summary>詳細</summary>
    
### サンドイッチマウントで共通する注意事項
- トッププレートはマイコン部分のでっぱりを収めるように該当部分を少し薄くしてあります。
そのため、印刷時にキーキャップが乗る面がビルドプレートに面するように向きを変更してください。
- プリントするパーツ以外にm2ねじ24本と7mmスペーサ12個が必要となります。

### 親指クラスタにMXスイッチを使用するケース
データ画保管先は[こちら](/case/sandwich_case/mx_thumb_sandwichcase)<br>
3Dプリントするデータは以下の通りです。
| 左右 | データ名 | 説明  |
| ---- | ---- | ---- |
| 左 | left_topplate.obj | 左手用トッププレート |
| 左 | left_bottomplate.obj | 左手用ボトムプレート |
| 右 | right_topplate.obj | 右手用トッププレート |
| 右 | right_bottomplate.obj | 右手用ボトムプレート |

### 親指クラスタにChoc v2スイッチを使用するケース
![chocv2_thumb_case](/image/chocthumb.png)

データ画保管先は[こちら](/case/sandwich_case/chocv2_thumb_sandwichcase)<br>
3Dプリントするデータは以下の通りです。
| 左右 | データ名 | 説明  |
| ---- | ---- | ---- |
| 左 | left_choc_plate.obj | 左手Chocスイッチ用トッププレート |
| 左 | left_mx_plate.obj | 左手MXスイッチ用トッププレート |
| 左 | left_bottom_plate.obj | 左手用ボトムプレート |
| 右 | right_choc_plate.obj | 右手Chocスイッチ用トッププレート |
| 右 | right_mx_plate.obj | 右手MXスイッチ用トッププレート |
| 右 | right_bottom_plate.obj | 右手用ボトムプレート |

### サンドイッチマウントケース用34mmトラックボールケース
- 34mm_trachball_case_forsandwichcase.obj

トラックボールケースデータは[こちら](/case/sandwich_case/34mm_trackball_case_forsandwichcase.obj)から

ZaruBallでは独自のトラックボール基板を採用しています。keyballやroBa, moNaのトラックボールケースは使用できません。<br>
トラックボールケースに2mmのセラミックボールを挿入してください。ドライバ―の裏側などで強く押し込むことで圧入できます。<br>
</details>