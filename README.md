# DrasticInputSourceStatus kawa-改造版

アプリケーションのダウンロード:
- [MacOS10.6はここ！](http://mitsuakikawamorita.com/software/DrasticInputSourceStatus/DrasticInputSourceStatus-3.1.2-MacOS10.6.dmg "app")
- [MacOS10.8はここ！(10.7もたぶんここ)](http://mitsuakikawamorita.com/software/DrasticInputSourceStatus/DrasticInputSourceStatus-3.1.2-MacOS10.8.dmg "app")

takezo氏制作の、IMEの状態によりメニューバーの色が変わるツール、DrasticInputSourcesStatusを少しいじって、画面全体で色が変化するようにしてみました。
私kawa-は元ソースを9行ぐらいしかいじっていませんので、takezo氏に圧倒的感謝！

## System requirements
Mac OS X 10.6 or higer.

## How to build

###Requirements:
* OS X 10.6
* Xcode 4.3+
* Command Line Tools for Xcode

### Step1: Getting source code

Execute a following command in Terminal.app.

<pre>
git clone --depth 10 https://github.com/ka-w-a/DrasticInputSourceStatus.git
</pre>

### Step2: Building a package

Execute a following command in Terminal.app.

<pre>
cd DrasticInputSourceStatus
make package
</pre>

Then, DrasticInputSourceStatus-3.1.2.dmg has been created in the current directory.
It's a distributable package.

### make package に失敗するとき
Mac OS 10.8 だとたぶん失敗します。そのときは、.xcodeprojをXcodeで開いて、真ん中上の、「Project」というところをクリックしますと、左の方にウィンドウが出ます。そして、Validate Project Settingってところをクリックしますとまたウィンドウが出ますので、Perform Changesを押して、Enableを押します。そして左上のRunを押して動作確認をしてから、make packageを再度行うと成功すると思います。
