# DrasticInputSourceStatus ka-w-a改造版
takezo氏制作の、IMEの状態によりメニューバーの色が変わるツール、DrasticInputSourcesStatusを少しいじって、画面全体で色が変化するようにしてみました。
私ka-w-aは元ソースを9行ぐらいしかいじっていませんので、takezo氏に圧倒的感謝！

-----

## System requirements
Mac OS X 10.6 or higer.

-----

## How to build

###Requirements:
* OS X 10.7
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

