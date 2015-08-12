# vagrant-ansible-wordpress-wordmove

WordPressサーバを構築するAnsible Playbookです。
開発環境を構築するときにWordmoveをインストールします。
本番環境を構築後、開発環境のWordmoveを使うことで開発と本番の同期が可能になります。

必要なソフトウェア
・Ansible

インストールされるソフトウェア
・MySQL5.6
・Nginx
・PHP5.6
・PHP-FPM
・WordPress

開発環境にのみインストールするソフトウェア
・Ruby2.1
・WordMove

本番環境にのみインストールするソフトウェア
・git
・logmon

使い方
$ vagrant up
$ ansible-playbook wordpress.yml -i hosts.development
$ curl http://dev.www.example.com/blog/

Copyright (c) 2015 <a href="http://boomil.com">boomil</a>
