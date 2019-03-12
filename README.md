# [MySQL management tool for VSCode](https://marketplace.visualstudio.com/items?itemName=poreklo.vscode-mysql)

[![Marketplace Version](https://vsmarketplacebadge.apphb.com/version-short/poreklo.vscode-mysql.svg)](https://marketplace.visualstudio.com/items?itemName=poreklo.vscode-mysql) [![Installs](https://vsmarketplacebadge.apphb.com/installs-short/poreklo.vscode-mysql.svg)](https://marketplace.visualstudio.com/items?itemName=poreklo.vscode-mysql) [![Rating](https://vsmarketplacebadge.apphb.com/rating-short/poreklo.vscode-mysql.svg)](https://marketplace.visualstudio.com/items?itemName=poreklo.vscode-mysql) [![Build Status](https://travis-ci.org/poreklo/vscode-mysql.svg?branch=master)](https://travis-ci.org/poreklo/vscode-mysql)

> Note: This tool forked from [MySQL (Jun Han)](https://marketplace.visualstudio.com/items?itemName=formulahendry.vscode-mysql).
>
> major changes:
>
> * add support for `DELIMITER` operator (can be switched by parameter `enableDelimiterOperator`)
> * update to support future vscode versions
>
> minor changes you can see in the [changelog](/CHANGELOG.md)

## Features

* Manage MySQL Connections (support SSL connection)
* List MySQL Servers
* List MySQL Databases
* List MySQL Tables
* List MySQL Columns
* Run MySQL Query

## Usage

* To add MySQL connection: in Explorer of VS Code, click "MYSQL" in the bottom left corner, then click the `+` button, then type host, user, password, port and certificate file path (optional) in the input box.

![connection](images/connection.png)

* To run MySQL query, open a SQL file first then:
  * right click on the SQL file, then click `Run MySQL Query` in editor context menu (Note: you could also run the selected SQL query)
  * or use shortcut `Ctrl+Alt+E`
  * or press `F1` and then select/type `Run MySQL Query`

![run](images/run.png)

* To create a new MySQL query or change active MySQL connection (You could see active MySQL connection in status bar):
  * right click on a MySQL server, then click `New Query`
  * or right click on a MySQL database, then click `New Query`

![newquery](images/newquery.png)

## Settings

* `vscode-mysql.maxTableCount`: The maximum table count shown in the tree view. (Default is **500**)
* `vscode-mysql.enableDelimiterOperator`: Enabling or disabling support for `DELIMITER` operator. If you execute large MySQL scripts without delimiter operator you may want to disable this function to improve performance. (Default: **True**)
* `vscode-mysql.keepResultWindow`: Keeps the result when switching tabs. Enabling this option increases memory usage. (Default: **False**)

## Change Log

See Change Log [here](/CHANGELOG.md)

## Issues

Currently, the extension is in the very initial phase. If you find any bug or have any suggestion/feature request, please submit the [issues](https://github.com/poreklo/vscode-mysql/issues) to the GitHub Repo.
