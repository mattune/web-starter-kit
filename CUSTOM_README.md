# Web Starter Kit - Matsuda Custom

## CSS

### 方針
- 基本的にmain.scssで全てのscssを読み込む。  
- ページ固有のcssを作る時はmain.scssと同列に置く  
ex) about.scss 等
- 基本的にPCファースト、必要があればSPファースト  
  - 全画角用のCSS → PC用のCSS → （必要があればタブレット用のCSS） → SP用のCSS の順番で読み込む


### 変更点
- _libフォルダを追加  
→ swiperとかのcssはここに入れる

- _commonから_moduleに名前変更  
→ サイト共通のcssをcommonにしたかったので、sass用のパーツはmoduleにした

- moduleに_parts.scssを追加  
→ わざわざcssを書きたくないようなちょっとしたパーツ用  
　 余白調整とか文字サイズとか

- _function.scssを_mixin.scssと結合  
→ 分けるほど色々な機能を書かないので

- _mixin.scssに毎回使う記述を追加  
→ メディアクエリとイージング周り

- _config.scssに毎回使う記述を追加  
→ 画面サイズやカラー等


---


## Javascript

### 方針
特にこだわり無し  
あえて言うなら、jQueryはまだなんやかんや使えるので入れておきたい

### 変更点
- libsにpluginsフォルダを追加  
→ 主にjQueryプラグイン用

- 