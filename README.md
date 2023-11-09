# LobbyReveal
Lobbyで味方を明らかにできるツールです    
手順１ wiresharkの設定    
wiresharkをインストールして、環境変数のPATHにWiresharkのインストールフォルダを追加して、コマンドラインでtsharkが使えるようにしてください     
手順２ 変数の設定     
22行目のcapture_interface_idにコマンドラインでtshark -Dとうち、イーサネットの番号をいれてください     
23行目のSSLKEYLOGFILEPATHにLeagueClientSettings.yamlのパスをいれてください  デフォルトの場所はC:\Riot Games\League of Legends\Logs\GameLogs\LeagueClientSettings.yaml    

これで準備完了です。
なぜか40%ぐらいの確率でしか味方の情報が入った通信を取得できないので正常に作動するかは運です
