# supabaseを使ったflutterアプリのサンプル  
  
# intro
supabaseに触れるためにflutterアプリを作成してみる  
実装する機能はログイン・ログアウト・新規登録  

参考に使ったサイト  
https://medium.com/geekculture/flutter-authentication-flow-with-supabase-opensource-firebase-alternative-438646c5703a  

# supabase の設定  
app.supabase.io にアクセスしてログインをします。  
新規プロジェクトからプロジェクトを作成します。（データベースが起動するまで時間がかかります。)

Authentication→Settings→Generalから  
処理を簡単にするためにDisable email confirmationsを有効化します。  

次にAPI周りの情報をコピーします  
Settigs→API→Configから  
URLとanon publicに書いてあるKeyをコピーします  

lib/main.dartの13,14行目付近のSUPABASE_URLとSUPABASE_ANON_KEYを書き換えます。  

````:bash
#実行したコマンド
flutter pub add supabase
flutter pub add get_it
flutter pub upgrade supabase
flutter pub add shared_preferences

# flutter pub get
````

シミュレータ等を起動してflutter runを実行します。

````:bash
open -a Simulator
flutter run
````


