
| Ansible共通コンソールのメニュー一覧を以下に記述します。


.. list-table::  Ansible共通コンソール メニュー/画面一覧
   :widths: 2 6 20
   :header-rows: 1
   :align: left

   * - No
     - メニュー・画面
     - 説明 
   * - 1
     - 機器一覧 
     - 作業対象ホストの情報をメンテナンス(閲覧/登録/更新/廃止)できます。 
   * - 2
     - インターフェース情報 
     - | Ansible Core、Ansible Automation Controllerサーバのどちらを実行エンジンとし構築作業をするか選択をします。
       | ITAシステム・Ansible driverサーバと実行エンジンのサーバが共有するディレクトリのパスおよび、実行エンジンのサーバへの接続インターフェース情報を管理します。
   * - 3
     - Ansible Automation Controllerホスト一覧 
     - Ansible Automation ControllerのRestAPI実行に必要な情報、および構築資材をAnsible Automation Controllerにファイル転送するために必要な情報を管理します。
   * - 4
     - グローバル変数管理
     - Playbookや対話ファイルなどで共通利用する変数（以降、グローバル変数と称す）と具体値を管理します。 
   * - 5
     - ファイル管理 
     - Playbook内の各モジュールで使用する素材ファイルと埋め込み変数を管理します。 
   * - 6
     - テンプレート管理
     - Playbook内のtemplateモジュールでなどで使用するテンプレートファイルと埋め込み変数を管理します。  
   * - 7
     - 共通変数利用リスト (※1)
     - テンプレート管理、ファイル管理、グローバル管理に登録されている変数をどの素材(ロール)で使用しているかを閲覧できます。
   * - 8
     - 管理対象外変数リスト (※1)
     - | ロールパッケージ管理のデフォルト変数定義やテンプレート管理の変数定義で定義している変数で、代入値自動登録の変数一覧に表示したくない変数をメンテナンス(参照/更新/廃止/復活)できます。
       | 変数名は正規表記で記載できます。
       | (例) ansible_* \*:ワイルドカード 
       | ansible\_[0-9a-zA-Z\_]\*  

.. note:: | ※1 非表示メニューは、バックヤード機能でデータの登録・更新を行うメニューです。
   | Ansible Driver機能をインストールした状態では表示されないメニューに設定されています。
   | 非表示メニューを表示するには、:menuselection:`管理コンソール-->ロール・メニュー紐付管理` で各メニューの復活処理を行います。詳細は :doc:`../it_automation_base/management_console` を参照してください。


