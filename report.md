---
title: 低軌道における宇宙農場のデブリの影響
tags: Debri
author: nanbuwks
slide: false
---
# アブストラクション

宇宙農業を行うには、ISS などと比較しはるかに大きなサイズの宇宙設備が必要となる。断面積も膨大なものとなり、デブリのヒットによる影響が甚大となる。本稿では、宇宙農場におけるデブリの確率の計算、および妥当な対策について述べる。

# 想定

宇宙での生活人口が100人超えた頃から自給体制を作る必要が出てくる。更に1000人規模で自給が軌道に乗った頃を想定すると、生活に必要な炭素の半分を再利用分で賄うぐらいで想定する。
![text](images/carboncycle.png)

そのような宇宙農場を作るとなると、デブリ
@bushoucow さんの考察「SpaceFarmProject」によると、人間一人を養うのに直径10mのバルーン100基ぐらいが必要となる。

その場合、デブリ被害はかなり大きなこととなる。
その具体的な数値を導き出してみよう。

## 「きぼう」モジュールを農場モジュールにした場合

宇宙食料生産の話を 1000人分で想定すると 床面積 1.1平方km と容積 330kL となるが、それをを軌道上で作るとなると、どういった施設が必要か? 最初の考察として、 ISSモジュールと同じもので作ると考える。ISS は雑多なモジュールで構成されているが、そのうちの「きぼう」の場合。

「きぼう」は6つの要素があり、そのうちのストレージの役割を持つ船内保管室が宇宙農場に最も近いものと考えることができる。「きぼう」の船内保管室は 直径、全長共に4.2m の円筒形、質量は4.2トン。これと同じ大きさで農場モジュールを作るとして、内部に同心円筒状にジャガイモ育成パレットを3段並べて 100m^2 としLEDで照明、中心に30リットルの酵母培養槽。パレットや培養槽、栽培マシン、水、作物などの質量を農場モジュール1つあたり10トンとすると、1人あたり農場モジュールは10基。
1000人分だと農場モジュールが1万基必要。相当な数量になる。


## 「きぼう」モジュール1万基の打ち上げコスト


さて農場モジュールに話を戻して、これを建設するとするとデブリ対策込で1基16トン、1万基で16万トン。
これを、 SPACEX 社の Falcon9 で打ち上げるとすると7300回の打ち上げが必要。
Falcon9 の費用は "CAPABILITIES & SERVICES"[1] で明らかにされており、 STANDARD PAYMENT PLAN で 6975万ドルとなっている。 7300打ち上げると5100億ドル。1000人の食料の半分を賄うにはコストがかかりすぎる。
したがって、このコストをいかに削減するかが問題となる。最も削減に寄与するのはトンあたりの打ち上げ費用が下がればよく、SPACEX 社の次期大型ロケットである SUPERHEAVY が実用化すればかなりコストダウンになる。しかしながら本稿ではトンをいかに削減するかを検討することにする。
「きぼう」モジュールの質量は4.2トンとなっているのだが、どうしてそれだけの重量が必要なのであろうか。

# デブリ対策


さてここで、「きぼう」船内保管室 のデブリ対策はどのようになっているだうか。厚み約10cmの シールド・バンパー・与圧壁で構成とのことである。[2]
![text](images/kiboshild.png)
Wikipedia の数字などからざっと計算すると、10年間軌道上で運用した場合のデブリやメテオロイドによる貫通確率は1%以下ぐらいとなる。これを1万基とすると1年間に100基は貫通されてしまうことになる。しかしながら衝突面の方向は偏りがあるために、そちらに向けて配列などを工夫すれば例えば 衝突面 に質量シールドを展開、その影に10基カスケードに配置する工夫をするとなると衝突確率は1/10 にとなることができる。このようにいろんな工夫でデブリの被害を減らすことができる。

# デブリのデータ


さきほどは衝突面の方向に偏りがあるということから質量シールドの展開などの方法を紹介したが、そのほかにデブリは高度などによっても変化する。
基本的な情報のいくつかを以下のように把握したい。

## 高度によるデブリの密度


"地球軌道を取 り巻 くデ ブリ 環境の現状"[2]

Page553 において10cm以上のデブリを含む人工宇宙物体について 2002 年のデータと推察される以下のデータがある。

![text](images/debridencity.png)

グラフのうち、恐らく全高度においてピークを除く部分の半数以上がデブリとなる。その仮定の上で、高度40000km以上だとかなりデブリが減ることになる。測位衛星などに使われる高度20000kmと静止軌道である高度36000kmにピークがあるほかは高度10000km〜320000km程度はあまり変化がなく、高度10000k以下はかなりデブリが混雑するだろうことがわかる。そのうちでも、高度800kmと1400km付近にピークがあり、ここは避けるべきであろう。ISSなどが運用されている高度400km以下と、高度1800km以上が望ましいことがわかる。
高度2000kmまでは低軌道(LEO)として区分されており、打ち上げコストのかからないLEOの範囲内だと高度400km前後、および、高度1800km〜2000kmが候補地となる。

## デブリの大きさと数

先の資料は 10cm 以上の物体の密度グラフであったのだが、10cmよりも小さな大きさのデブリは相当数が増えることになる。英語版Wikipedia [3] 2024・6・9時点の記述では、

> Size and numbers
As of January 2019 there were estimated to be over 128 million pieces of debris smaller than 1 cm (0.39 in), and approximately 900,000 pieces between 1 and 10 cm. The count of large debris (defined as 10 cm across or larger[44]) was 34,000 in 2019,[8] and at least 37,000 by June 2023.[45] The technical measurement cut-off[clarification needed] is c. 3 mm (0.12 in).[46]


とあり、目安として直径サイズ1/2ごとに10倍に増えるととらえるのが妥当と考える。
そして、10cm 以上のデブリは軌道が把握しやすく回避などを行うことができるのであるが、小さなデブリは存在が把握できない割合が多くなり、それらの衝突リスクが重要となる。
# デブリ防御

デブリが衝突した場合はどのようなことが起こるだろうか。
例えばニューナンブの拳銃弾の初速が 0.2km/s 程度、ライフル弾が少口径高速弾と言われる 5.56mm NATO弾で0.9km/s 、チート級APFSDSである3BM69 でも2km/s 程度である。宇宙軌道速度は 5km/s 、 10km/s という速度がいかに脅威となるかがわかる。
ここで10km/s のデブリへの防御を考える。この程度だと運動エネルギーによって衝突体・被衝突体ともに接触した箇所は流体となる。したがってデブリに対しての装甲はモース硬度とか一切関係なくなり、反発係数 e=0 とした作用反作用の運動方程式を解くことになる。 

このような場合、装甲は質量による防護が卓越することになる。驚くべきことにこのような状態ではデブリの速度は侵徹深さにはあまり関係がなくなり、デブリの奥行きと密度に依存することになる。例えばデブリの奥行きが1cm として、同じ密度の装甲とすると同じ1cm の厚さで貫通は防ぐことができ、あとは弾着点からの運動量や衝撃波に耐える裏打ちがあればいいことになる。
ISSのきぼう実験棟はメインの外壁装甲以外に衝突リスクの高いところはスペースドアーマー的にデブリバンパーがある。
そのようにして防御できるのは、直径奥行き1cm程度のデブリでありそれ以上になる場合、回避できなければ貫通してしまう。その場合の衝突確率は10年で3%とされる。

装甲の能力は、RHA  (均質圧延鋼装甲) 換算で表すことが多く、例えばアルミの奥行き1cm に対応する装甲は RHA 3.4mm 厚となる。しかしながら 1m^2 で 27kg となり質量が嵩んでしまう。これは鉄だから重いというわけではなく材料を変えたとしても質量装甲なので必ず  1m^2 あたり 27kg 必要となる。
ではこれを軽量化するにはどのようにすればよいだろうか。 例えば装甲から離して薄い板を置き、デブリを衝突衝撃波で粉砕してしまい装甲に至る奥行き方向の質量を減らすデブリバンパーという方法や、装甲板を必需品であるがデブリヒットされてもダメージの少ないものに置き換えてしまう、などいろんなアイデアがある。デブリヒットされても良いものの例として、例えば水タンクを小分けしてロシア戦車の爆発反応モジュールのように宇宙船表面に貼り付け、デブリで損傷したものは破棄交換するなどが考えられる。この問題については良い解決策を期待したい。


# 衝突確率



デブリの衝突速度について。色んなパターンがあるのではあるが、今回は円軌道を持つもの同士の衝突に絞って考察する。デブリ発生時に与えられた速度ベクトルが大きなものはほとんど地球に落ちてしまうので、円軌道から大きく外れてないデブリが多いだろうという予測に基づくものである。
ここでも、ISS を例として計算を行う。ISS の軌道傾斜角はバイコヌール基地を使う関係上 51.6度に設定されている。まず最初にその ISS と同じ51.6度と軌道傾斜角0度のデブリとの衝突。
軌道速度を v とすると衝突相対速度V は V=2v sin(51.6/2) なので 6.7km/s。
![text](images/debriorbit.png)
軌道傾斜角両方とも 51.6度の物体だけれども位相のずれが0度の場合は、衝突相対速度は0 。
さて、実際の宇宙物体の軌道傾斜角はどうなっているかというと、
"ORBITAL DEBRIS
National Academies of Sciences, Engineering, and Medicine. 1995. Orbital Debris: A Technical Assessment. Washington, DC: The National Academies Press. https://doi.org/10.17226/4765." Page66 [4]

によると、
によるとほとんどが60度から105度の間に集中している。
![text](images/debriorbitdegree.png)
これらのことから、荒っぽい仮定として危険な速度を5km/s 以上とし、位相と傾斜角によって危険な速度を持つデブリは総数の半分と考える。もちろん、デブリ対策によってどれだけの速度が脅威になるかは変わることになる。
# 求められる宇宙農場のデブリ対策

今までの考察から、宇宙農場モジュールのデブリへの衝突頻度は以下で計算できる。

( 宇宙農場投影面積 * (地球半径+軌道⾼度) * 2 * 3.14 ) * デブリ密度 / 周回時間(1時間) * 危険速度率 = [ ]衝突/秒

LEOにおけるデブリ密度の最新データは以下が使用できる。 
"History of On-orbit Satellite Fragmentations, 16th Edition"[5] Page23
![text](images/debrialtitude.png)

高度400kmで考えると密度が1.5E-08km^3となり、危険速度率が0.1 とすると、10年間で0.01%。
これは10cm以上のデータであろうから、1.25cm以上のもので考えると (10)^(log2(10/1.25))倍で10年間で10%。
先の Wikipedia の数字から考えるとかなり大きくなるのであるが、それについては補正が必要となる可能性もある。


# 参考文献

[1] https://www.spacex.com/media/Capabilities&Services.pdf

[2]https://www.jstage.jst.go.jp/article/sicejl1962/41/8/41_8_551/_pdf


[3]https://en.wikipedia.org/wiki/Space_debris


[4]https://nap.nationalacademies.org/read/4765/chapter/6#68

[5] https://www.orbitaldebris.jsc.nasa.gov/library/HOOSF_16e.pdf

このほか、低軌道のデブリ評価について。ISS実験棟「きぼう」のPNP( 非貫通確率、Probability of No Penetration）の数値の前提はこちらを見るのが良さそう。『 「国際宇宙ステーションの日本実験棟「きぼう」(JEM)に係る安全対策の評価のための基本指針」に対する安全検証結果』