# F's Plugins
Adone After EffectsのEffectsPlugin集のソース一式とバイナリです。  
  
昔から趣味でコツコツと作っていたものです。  
趣味といっても僕自身日本のアニメ制作者なので業務に使ってます。
  
CC2019用からgithubでバイナリーの配布も行います。
**_DL_windowsbinary**フォルダの中に入っています。  

基本的に配布しているバイナリーはwindows用 のみです。  
Mac用はありません。  
  
* [Fsplugins2020726.zip](https://bit.ly/2OXxZJj)  
7月26日版です。SDKをCC2020に変えてビルドしただけのものです。しばらく使ったら正式版にします。

# 変更点
2020/07/26  
CC2020 SDKに変更。  
  
2020/03/20  
CC2019 SDKに変更。  
数が多くなって使いにくくなったので、カテゴリーを整理しました。  
* F's Plugins-Cell  
 アニメのスムージングなしのセルをターゲットにしたものです。
* F's Plugins-Channel  
 チャンネル操作系です。
* F's Plugins-Colorize  
 色を付けるものです。
* F's Plugins-Draw  
 描画系のものです。
* F's Plugins-Filter  
 フィルターエフェクト系です。
* F's Plugins-Noise  
 ノイズフィルタ系です。
* F's Plugins-{Legacy}  
 もう使って欲しくない。或いは使い道のないものです。  
 紙飛行機作成補助プラグインとか
### 追加プラグイン
* F's EdgeLine-Hi.aex  指定した2色の境界に線を描きます。その時描く向きを指定できます。
* F's Flare.aex 白黒マスクにグローを付けます。透過光です。
* F's graytoneToColorize.aex 簡易コロラマです。ゴールド処理やサーモグラフ処理に使います。
* F's PixelExtend.aex 指定した色を指定した方向に膨張させます。
* F's Posterization8bit.aex ポスタリゼーションです。標準と違って内部は8bit処理です。
* F's Scanline.aex スキャンライン。昔の古いパソコンの偶数列が黒いラインの状態ができます。
* F's YuvControl.aex YUV版のRGBAコントロールです。

# 開発環境
Visual studio 2017 Community 2017 C++
AfterEffectsSDK CC2019
SDKはCC2019を使用していますが、CS4/CS6のSDKでもbuild可能です。

# Setup
プロジェクト等はSDKフォルダ内のExampleフォルダ内へ配置してください。

こんな感じです。

        /AfterEffectsSDK CC2019    
        └─Examples  
            ├─AEGP  
            ├─Effect  
            ├─F's PluginsProjects  
            │  ├─AlphaFix  
            │  ├─AlphaThreshold  
            │  ├─AnimatedNoise  
            <省略>  
            │  ├─PluginSkeleton  
            <省略>  
            │  ├─whiteInOut  
            ├─GP 
            ├─Headers  
            ├─Resources  
            ├─Template  
            ├─UI  
            └─Util  

# 使い方

SDKはCC2018/CC2019を想定していますが、CS6及びCC2019までのSDKでビルド可能です。
  
F's PluginsProjectsフォルダを各バージョンのExamplesフォルダに移動すればできます。
  

構成でPelease/Relese-MTとありますが、ランタイムライブラリのスイッチ(/MT/MD)が違うものです。それ以外は同じです。  
PluginのBinaryはoutAEXDに書き出されます。  

PluginのBinaryはAfter EffectsのPlug-insへコピーしてください。  
  
例)  
"C:\Program Files\Adobe\Adobe After Effects CC 2019\Support Files\Plug-ins"


# ライセンス

This software is released under the MIT License, see LICENSE. 
  
このソースコードを使用する時はMITライセンスに準じてください。  
独自にビルドして映像制作使う場合は、使用プラグインリスト等にここのurl(https://github.com/bryful)を入れてもらえればOKです（まぁ入れなくても僕は気にしません）  

このプログラムを映像制作に使用した場合も特に制限ありません。一応MITライセンスの条件である著作権表示および本許諾表示として  

**プラグイン協力 bry-ful**  

とクレジットしてくれると嬉しいです（これは強制ではありませんので、基本的に無断使用でかまいません）

P関係のゲーム会社の方へ 
使用に関しては特に制限ありません。許諾も必要ありません。使用料も発生しません。 
これは今後絶対に変わりません。
  
# Authors

twitter:[bryful](https://twitter.com/bryful)  
github :[bryful](https://github.com/bryful)  
bryful@gmail.com  

# References

