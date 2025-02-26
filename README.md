# Laravel 12 + Livewire Study Project

このプロジェクトは、Laravel 12 と Livewire を利用した開発環境の学習用サンプルです。特に、Livewire コンポーネントのルーティングを簡素化するために「Volt」を導入しており、コンポーネントベースの設計や動的 UI の実装方法を学習することが目的です。

## プロジェクト概要

- **フレームワーク:** Laravel 12
- **UI ライブラリ:** Livewire
- **ルーティング:** Volt を使用して Livewire コンポーネントに直感的なルーティングを実現
- **学習対象:** Laravel の基本構造、Livewire を用いたリアクティブなコンポーネント、及び Volt によるルート管理

## セットアップ方法

1. リポジトリをクローンします。
2. `composer install` を実行し、依存関係をインストールします。
3. `.env` ファイルを作成し、適切な設定を行います。
4. `php artisan migrate` でデータベースのマイグレーションを実行します。
5. `php artisan serve` でローカル開発サーバーを起動します。

## ディレクトリ構成

以下は、このプロジェクトの主要なディレクトリ構成の一例です。


. ├── app │ ├── Console │ ├── Exceptions │ ├── Http │ │ ├── Controllers │ │ └── Livewire # Livewire コンポーネントを配置するディレクトリ │ ├── Models │ └── Providers ├── bootstrap ├── config ├── database │ ├── factories │ ├── migrations │ └── seeders ├── public │ └── index.php # アプリケーションのエントリーポイント ├── resources │ ├── css │ ├── js │ └── views # Blade テンプレート用のディレクトリ │ ├── welcome.blade.php │ ├── dashboard.blade.php │ └── livewire # Livewire 用のビューを配置 ├── routes │ ├── web.php # Web ルート (Volt ルートもこちらで定義) │ └── api.php ├── storage ├── tests └── vendor

## ルーティングについて

このプロジェクトでは、通常の Laravel ルーティングに加えて、Volt を利用したルート定義を行っています。例えば、以下のように Livewire コンポーネントへのルートが定義されています。

```php
Volt::route('settings/profile', 'settings.profile')->name('settings.profile');
---

上記の README サンプルは、Laravel 12 を使用した Livewire の学習プロジェクトとしての概要とディレクトリ構成の例を示しています。これを元に、プロジェクトの内容に合わせて適宜カスタマイズしてください。
