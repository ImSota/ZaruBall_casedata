# ZaruBall用3Dプリントデータ
ZaruBallは現状サンドイッチマウントのみに対応しています。<br>
2ピースケース、25mmボール用トラックボールケースを今後設計予定です。
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
データ保管先：
[chocv2_thumb_sandwichcase](chocv2_thumb_sandwichcase)<br>

プリントする3Dモデル：
- right_choc_plate.obj (右手Chocスイッチ用トッププレート)
- right_mx_plate.obj (右手MXスイッチ用ボトムプレート)
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
