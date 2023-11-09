# LobbyReveal
Lobbyで味方を明らかにできるツールです    
## 手順１ wiresharkの設定    
wiresharkをインストールして、環境変数のPATHにWiresharkのインストールフォルダを追加して、コマンドラインでtsharkが使えるようにしてください      
Windowsの場合:   

tsharkの実行可能ファイルのパスを取得します。通常、Wiresharkがインストールされているディレクトリにあります。デフォルトのパスは通常 C:\Program Files\Wireshark です。

スタートメニューから「環境変数を編集」を検索し、システムの環境変数を編集するための「環境変数」ボタンをクリックします。

「システム環境変数」のセクションで、Pathという名前の環境変数を選択し、編集ボタンをクリックします。

「新規」ボタンをクリックし、tsharkの実行可能ファイルのディレクトリへのパスを入力します。複数のディレクトリを追加する場合は、それぞれをセミコロン (;) で区切ります。

すべてのダイアログを閉じ、設定を保存します。

新たに開いたコマンドプロンプトウィンドウで tshark コマンドを実行できるようになります。

## 手順２ 変数の設定     
22行目のcapture_interface_idにコマンドラインでtshark -Dとうち、イーサネットの番号をいれてください     
23行目のSSLKEYLOGFILEPATHにLeagueClientSettings.yamlのパスをいれてください  デフォルトの場所はC:\Riot Games\League of Legends\Logs\GameLogs\LeagueClientSettings.yaml    

これで準備完了です。
自動でロビー入室を検知するので、マッチ検索をかける時に起動しておいてください
なぜか40%ぐらいの確率でしか味方の情報が入った通信を取得できないので正常に作動するかは運です
