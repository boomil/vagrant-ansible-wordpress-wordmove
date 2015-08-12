# vagrant-ansible-wordpress-wordmove

## 概要

WordPressサーバを構築するAnsible Playbookです。
開発環境を構築するときにWordmoveをインストールします。
本番環境を構築後、開発環境のWordmoveを使うことで開発と本番の同期が可能になります。

## 関連するソフトウェア

### 必要なソフトウェア

* Ansible
* Vagrant

### インストールされるソフトウェア

* MySQL5.6
* Nginx
* PHP5.6
* PHP-FPM
* WordPress

### 開発環境のみインストールされるソフトウェア

* Ruby2.1
* WordMove

### 本番環境のみインストールされるソフトウェア

* git
* logmon

## 使い方

	$ vagrant up
	$ ansible-playbook wordpress.yml -i hosts.development
	$ curl http://dev.www.example.com/blog/

Copyright (c) 2015 <a href="http://boomil.com">boomil</a>
