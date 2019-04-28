<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [Python・機械学習まとめ](#python%E3%83%BB%E6%A9%9F%E6%A2%B0%E5%AD%A6%E7%BF%92%E3%81%BE%E3%81%A8%E3%82%81)
  - [詳細！Python 3 入門ノートまとめ](#%E8%A9%B3%E7%B4%B0python-3-%E5%85%A5%E9%96%80%E3%83%8E%E3%83%BC%E3%83%88%E3%81%BE%E3%81%A8%E3%82%81)
    - [ステートメントとは](#%E3%82%B9%E3%83%86%E3%83%BC%E3%83%88%E3%83%A1%E3%83%B3%E3%83%88%E3%81%A8%E3%81%AF)
    - [ステートメントを途中で折り返したいとき](#%E3%82%B9%E3%83%86%E3%83%BC%E3%83%88%E3%83%A1%E3%83%B3%E3%83%88%E3%82%92%E9%80%94%E4%B8%AD%E3%81%A7%E6%8A%98%E3%82%8A%E8%BF%94%E3%81%97%E3%81%9F%E3%81%84%E3%81%A8%E3%81%8D)
    - [値の区切り文字、改行を指定する](#%E5%80%A4%E3%81%AE%E5%8C%BA%E5%88%87%E3%82%8A%E6%96%87%E5%AD%97%E6%94%B9%E8%A1%8C%E3%82%92%E6%8C%87%E5%AE%9A%E3%81%99%E3%82%8B)
    - [round](#round)
    - [２進数、８進数、１６進数](#%EF%BC%92%E9%80%B2%E6%95%B0%EF%BC%98%E9%80%B2%E6%95%B0%EF%BC%91%EF%BC%96%E9%80%B2%E6%95%B0)
    - [複素数](#%E8%A4%87%E7%B4%A0%E6%95%B0)
    - [数値演算子「//」](#%E6%95%B0%E5%80%A4%E6%BC%94%E7%AE%97%E5%AD%90)
    - [複数行の文字列](#%E8%A4%87%E6%95%B0%E8%A1%8C%E3%81%AE%E6%96%87%E5%AD%97%E5%88%97)
    - [[]で文字列を取り出す](#%E3%81%A7%E6%96%87%E5%AD%97%E5%88%97%E3%82%92%E5%8F%96%E3%82%8A%E5%87%BA%E3%81%99)
      - [部分文字列を抜き出す](#%E9%83%A8%E5%88%86%E6%96%87%E5%AD%97%E5%88%97%E3%82%92%E6%8A%9C%E3%81%8D%E5%87%BA%E3%81%99)
      - [ステップがある書式](#%E3%82%B9%E3%83%86%E3%83%83%E3%83%97%E3%81%8C%E3%81%82%E3%82%8B%E6%9B%B8%E5%BC%8F)
    - [ビット演算子](#%E3%83%93%E3%83%83%E3%83%88%E6%BC%94%E7%AE%97%E5%AD%90)
    - [型を調べる](#%E5%9E%8B%E3%82%92%E8%AA%BF%E3%81%B9%E3%82%8B)
    - [リテラルとリファレンス](#%E3%83%AA%E3%83%86%E3%83%A9%E3%83%AB%E3%81%A8%E3%83%AA%E3%83%95%E3%82%A1%E3%83%AC%E3%83%B3%E3%82%B9)
    - [mathモジュールに含まれる関数](#math%E3%83%A2%E3%82%B8%E3%83%A5%E3%83%BC%E3%83%AB%E3%81%AB%E5%90%AB%E3%81%BE%E3%82%8C%E3%82%8B%E9%96%A2%E6%95%B0)
    - [関数を指定して読み込む](#%E9%96%A2%E6%95%B0%E3%82%92%E6%8C%87%E5%AE%9A%E3%81%97%E3%81%A6%E8%AA%AD%E3%81%BF%E8%BE%BC%E3%82%80)
    - [大文字小文字の変換](#%E5%A4%A7%E6%96%87%E5%AD%97%E5%B0%8F%E6%96%87%E5%AD%97%E3%81%AE%E5%A4%89%E6%8F%9B)
    - [文字列を検索する](#%E6%96%87%E5%AD%97%E5%88%97%E3%82%92%E6%A4%9C%E7%B4%A2%E3%81%99%E3%82%8B)
      - [countメソッド](#count%E3%83%A1%E3%82%BD%E3%83%83%E3%83%89)
      - [findメソッド](#find%E3%83%A1%E3%82%BD%E3%83%83%E3%83%89)
    - [文字列を置換する](#%E6%96%87%E5%AD%97%E5%88%97%E3%82%92%E7%BD%AE%E6%8F%9B%E3%81%99%E3%82%8B)
    - [余分な文字を取り除く](#%E4%BD%99%E5%88%86%E3%81%AA%E6%96%87%E5%AD%97%E3%82%92%E5%8F%96%E3%82%8A%E9%99%A4%E3%81%8F)
    - [文字列に値を埋め込む](#%E6%96%87%E5%AD%97%E5%88%97%E3%81%AB%E5%80%A4%E3%82%92%E5%9F%8B%E3%82%81%E8%BE%BC%E3%82%80)
    - [値の書式設定](#%E5%80%A4%E3%81%AE%E6%9B%B8%E5%BC%8F%E8%A8%AD%E5%AE%9A)
    - [値の位置揃え](#%E5%80%A4%E3%81%AE%E4%BD%8D%E7%BD%AE%E6%8F%83%E3%81%88)
    - [if文](#if%E6%96%87)
    - [Falseとみなされる値](#false%E3%81%A8%E3%81%BF%E3%81%AA%E3%81%95%E3%82%8C%E3%82%8B%E5%80%A4)
    - [Pythonでの三項演算子の代わり](#python%E3%81%A7%E3%81%AE%E4%B8%89%E9%A0%85%E6%BC%94%E7%AE%97%E5%AD%90%E3%81%AE%E4%BB%A3%E3%82%8F%E3%82%8A)
    - [while文](#while%E6%96%87)
    - [break](#break)
    - [continue](#continue)
    - [while~else文](#whileelse%E6%96%87)
    - [range関数](#range%E9%96%A2%E6%95%B0)
    - [for文でのbreak](#for%E6%96%87%E3%81%A7%E3%81%AEbreak)
    - [for in ~ else](#for-in--else)
    - [例外処理](#%E4%BE%8B%E5%A4%96%E5%87%A6%E7%90%86)
      - [try + except + finally](#try--except--finally)
      - [例外オブジェクトによって処理を振り分ける](#%E4%BE%8B%E5%A4%96%E3%82%AA%E3%83%96%E3%82%B8%E3%82%A7%E3%82%AF%E3%83%88%E3%81%AB%E3%82%88%E3%81%A3%E3%81%A6%E5%87%A6%E7%90%86%E3%82%92%E6%8C%AF%E3%82%8A%E5%88%86%E3%81%91%E3%82%8B)
      - [try + except + except + else + finally](#try--except--except--else--finally)
      - [例外情報を調べる except as](#%E4%BE%8B%E5%A4%96%E6%83%85%E5%A0%B1%E3%82%92%E8%AA%BF%E3%81%B9%E3%82%8B-except-as)
    - [リスト](#%E3%83%AA%E3%82%B9%E3%83%88)
      - [list()](#list)
      - [リストのインデックスエラーを回避する](#%E3%83%AA%E3%82%B9%E3%83%88%E3%81%AE%E3%82%A4%E3%83%B3%E3%83%87%E3%83%83%E3%82%AF%E3%82%B9%E3%82%A8%E3%83%A9%E3%83%BC%E3%82%92%E5%9B%9E%E9%81%BF%E3%81%99%E3%82%8B)
      - [リストの末尾に要素を追加する](#%E3%83%AA%E3%82%B9%E3%83%88%E3%81%AE%E6%9C%AB%E5%B0%BE%E3%81%AB%E8%A6%81%E7%B4%A0%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%99%E3%82%8B)
      - [指定の位置に要素を挿入する](#%E6%8C%87%E5%AE%9A%E3%81%AE%E4%BD%8D%E7%BD%AE%E3%81%AB%E8%A6%81%E7%B4%A0%E3%82%92%E6%8C%BF%E5%85%A5%E3%81%99%E3%82%8B)
    - [リストの要素を削除する](#%E3%83%AA%E3%82%B9%E3%83%88%E3%81%AE%E8%A6%81%E7%B4%A0%E3%82%92%E5%89%8A%E9%99%A4%E3%81%99%E3%82%8B)
    - [指定の値を削除する](#%E6%8C%87%E5%AE%9A%E3%81%AE%E5%80%A4%E3%82%92%E5%89%8A%E9%99%A4%E3%81%99%E3%82%8B)
    - [split](#split)
    - [リストを連結する](#%E3%83%AA%E3%82%B9%E3%83%88%E3%82%92%E9%80%A3%E7%B5%90%E3%81%99%E3%82%8B)
    - [リストのスライス](#%E3%83%AA%E3%82%B9%E3%83%88%E3%81%AE%E3%82%B9%E3%83%A9%E3%82%A4%E3%82%B9)
    - [値やオブジェクト比較](#%E5%80%A4%E3%82%84%E3%82%AA%E3%83%96%E3%82%B8%E3%82%A7%E3%82%AF%E3%83%88%E6%AF%94%E8%BC%83)
    - [参照](#%E5%8F%82%E7%85%A7)
    - [リストの複製](#%E3%83%AA%E3%82%B9%E3%83%88%E3%81%AE%E8%A4%87%E8%A3%BD)
    - [リストの要素をソートする](#%E3%83%AA%E3%82%B9%E3%83%88%E3%81%AE%E8%A6%81%E7%B4%A0%E3%82%92%E3%82%BD%E3%83%BC%E3%83%88%E3%81%99%E3%82%8B)
    - [ソートした新しいリストを作る](#%E3%82%BD%E3%83%BC%E3%83%88%E3%81%97%E3%81%9F%E6%96%B0%E3%81%97%E3%81%84%E3%83%AA%E3%82%B9%E3%83%88%E3%82%92%E4%BD%9C%E3%82%8B)
    - [単純にリストの要素の並び順を逆順にしたい場合](#%E5%8D%98%E7%B4%94%E3%81%AB%E3%83%AA%E3%82%B9%E3%83%88%E3%81%AE%E8%A6%81%E7%B4%A0%E3%81%AE%E4%B8%A6%E3%81%B3%E9%A0%86%E3%82%92%E9%80%86%E9%A0%86%E3%81%AB%E3%81%97%E3%81%9F%E3%81%84%E5%A0%B4%E5%90%88)
    - [リストの要素をランダムにならべかえる](#%E3%83%AA%E3%82%B9%E3%83%88%E3%81%AE%E8%A6%81%E7%B4%A0%E3%82%92%E3%83%A9%E3%83%B3%E3%83%80%E3%83%A0%E3%81%AB%E3%81%AA%E3%82%89%E3%81%B9%E3%81%8B%E3%81%88%E3%82%8B)
    - [ソートで使う比較関数を指定する](#%E3%82%BD%E3%83%BC%E3%83%88%E3%81%A7%E4%BD%BF%E3%81%86%E6%AF%94%E8%BC%83%E9%96%A2%E6%95%B0%E3%82%92%E6%8C%87%E5%AE%9A%E3%81%99%E3%82%8B)
    - [for文でカウンタをつけて表示する](#for%E6%96%87%E3%81%A7%E3%82%AB%E3%82%A6%E3%83%B3%E3%82%BF%E3%82%92%E3%81%A4%E3%81%91%E3%81%A6%E8%A1%A8%E7%A4%BA%E3%81%99%E3%82%8B)
    - [for文で複数のリストを対象にする](#for%E6%96%87%E3%81%A7%E8%A4%87%E6%95%B0%E3%81%AE%E3%83%AA%E3%82%B9%E3%83%88%E3%82%92%E5%AF%BE%E8%B1%A1%E3%81%AB%E3%81%99%E3%82%8B)
    - [リスト内包表記](#%E3%83%AA%E3%82%B9%E3%83%88%E5%86%85%E5%8C%85%E8%A1%A8%E8%A8%98)
    - [条件式付きのリスト内包表記](#%E6%9D%A1%E4%BB%B6%E5%BC%8F%E4%BB%98%E3%81%8D%E3%81%AE%E3%83%AA%E3%82%B9%E3%83%88%E5%86%85%E5%8C%85%E8%A1%A8%E8%A8%98)
    - [indexメソッド](#index%E3%83%A1%E3%82%BD%E3%83%83%E3%83%89)
    - [個数を調べる](#%E5%80%8B%E6%95%B0%E3%82%92%E8%AA%BF%E3%81%B9%E3%82%8B)
    - [リストから要素をランダムに取り出したい場合](#%E3%83%AA%E3%82%B9%E3%83%88%E3%81%8B%E3%82%89%E8%A6%81%E7%B4%A0%E3%82%92%E3%83%A9%E3%83%B3%E3%83%80%E3%83%A0%E3%81%AB%E5%8F%96%E3%82%8A%E5%87%BA%E3%81%97%E3%81%9F%E3%81%84%E5%A0%B4%E5%90%88)
    - [tuple()を使って文字列を分解してタプルにする](#tuple%E3%82%92%E4%BD%BF%E3%81%A3%E3%81%A6%E6%96%87%E5%AD%97%E5%88%97%E3%82%92%E5%88%86%E8%A7%A3%E3%81%97%E3%81%A6%E3%82%BF%E3%83%97%E3%83%AB%E3%81%AB%E3%81%99%E3%82%8B)
    - [セット](#%E3%82%BB%E3%83%83%E3%83%88)
    - [セットに要素を追加する](#%E3%82%BB%E3%83%83%E3%83%88%E3%81%AB%E8%A6%81%E7%B4%A0%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%99%E3%82%8B)
    - [セットから要素を削除する](#%E3%82%BB%E3%83%83%E3%83%88%E3%81%8B%E3%82%89%E8%A6%81%E7%B4%A0%E3%82%92%E5%89%8A%E9%99%A4%E3%81%99%E3%82%8B)
    - [frozenset型のセット](#frozenset%E5%9E%8B%E3%81%AE%E3%82%BB%E3%83%83%E3%83%88)
    - [セットの集合演算](#%E3%82%BB%E3%83%83%E3%83%88%E3%81%AE%E9%9B%86%E5%90%88%E6%BC%94%E7%AE%97)
    - [セットの和集合](#%E3%82%BB%E3%83%83%E3%83%88%E3%81%AE%E5%92%8C%E9%9B%86%E5%90%88)
    - [セットの積集合](#%E3%82%BB%E3%83%83%E3%83%88%E3%81%AE%E7%A9%8D%E9%9B%86%E5%90%88)
    - [セットの差集合](#%E3%82%BB%E3%83%83%E3%83%88%E3%81%AE%E5%B7%AE%E9%9B%86%E5%90%88)
    - [セットの対称差集合](#%E3%82%BB%E3%83%83%E3%83%88%E3%81%AE%E5%AF%BE%E7%A7%B0%E5%B7%AE%E9%9B%86%E5%90%88)
    - [集合演算結果でセットの内容を更新する](#%E9%9B%86%E5%90%88%E6%BC%94%E7%AE%97%E7%B5%90%E6%9E%9C%E3%81%A7%E3%82%BB%E3%83%83%E3%83%88%E3%81%AE%E5%86%85%E5%AE%B9%E3%82%92%E6%9B%B4%E6%96%B0%E3%81%99%E3%82%8B)
    - [セット同士に共通要素があるかどうかを判定する](#%E3%82%BB%E3%83%83%E3%83%88%E5%90%8C%E5%A3%AB%E3%81%AB%E5%85%B1%E9%80%9A%E8%A6%81%E7%B4%A0%E3%81%8C%E3%81%82%E3%82%8B%E3%81%8B%E3%81%A9%E3%81%86%E3%81%8B%E3%82%92%E5%88%A4%E5%AE%9A%E3%81%99%E3%82%8B)
    - [セットの包含関係を調べる](#%E3%82%BB%E3%83%83%E3%83%88%E3%81%AE%E5%8C%85%E5%90%AB%E9%96%A2%E4%BF%82%E3%82%92%E8%AA%BF%E3%81%B9%E3%82%8B)
    - [タプル（キー, 値）のリストから辞書を作る](#%E3%82%BF%E3%83%97%E3%83%AB%E3%82%AD%E3%83%BC-%E5%80%A4%E3%81%AE%E3%83%AA%E3%82%B9%E3%83%88%E3%81%8B%E3%82%89%E8%BE%9E%E6%9B%B8%E3%82%92%E4%BD%9C%E3%82%8B)
    - [zip()を利用し、キーと値のリストを合わせて辞書にする](#zip%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%82%AD%E3%83%BC%E3%81%A8%E5%80%A4%E3%81%AE%E3%83%AA%E3%82%B9%E3%83%88%E3%82%92%E5%90%88%E3%82%8F%E3%81%9B%E3%81%A6%E8%BE%9E%E6%9B%B8%E3%81%AB%E3%81%99%E3%82%8B)
    - [キーワード引数を利用して辞書を作る](#%E3%82%AD%E3%83%BC%E3%83%AF%E3%83%BC%E3%83%89%E5%BC%95%E6%95%B0%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A6%E8%BE%9E%E6%9B%B8%E3%82%92%E4%BD%9C%E3%82%8B)
    - [初期値で辞書を作る](#%E5%88%9D%E6%9C%9F%E5%80%A4%E3%81%A7%E8%BE%9E%E6%9B%B8%E3%82%92%E4%BD%9C%E3%82%8B)
    - [setdefault()を利用して、キーがあればそのまま、なければ追加する](#setdefault%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A6%E3%82%AD%E3%83%BC%E3%81%8C%E3%81%82%E3%82%8C%E3%81%B0%E3%81%9D%E3%81%AE%E3%81%BE%E3%81%BE%E3%81%AA%E3%81%91%E3%82%8C%E3%81%B0%E8%BF%BD%E5%8A%A0%E3%81%99%E3%82%8B)
    - [update()を利用して他の辞書を更新する](#update%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A6%E4%BB%96%E3%81%AE%E8%BE%9E%E6%9B%B8%E3%82%92%E6%9B%B4%E6%96%B0%E3%81%99%E3%82%8B)
    - [delを利用して、指定のキーの要素を削除する](#del%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A6%E6%8C%87%E5%AE%9A%E3%81%AE%E3%82%AD%E3%83%BC%E3%81%AE%E8%A6%81%E7%B4%A0%E3%82%92%E5%89%8A%E9%99%A4%E3%81%99%E3%82%8B)
    - [辞書内包表記](#%E8%BE%9E%E6%9B%B8%E5%86%85%E5%8C%85%E8%A1%A8%E8%A8%98)
    - [dict.fromkeys()を利用して、同じ構造の辞書を作る](#dictfromkeys%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A6%E5%90%8C%E3%81%98%E6%A7%8B%E9%80%A0%E3%81%AE%E8%BE%9E%E6%9B%B8%E3%82%92%E4%BD%9C%E3%82%8B)
    - [pop()を利用して、指定したキーの値を取り出して、削除する](#pop%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A6%E6%8C%87%E5%AE%9A%E3%81%97%E3%81%9F%E3%82%AD%E3%83%BC%E3%81%AE%E5%80%A4%E3%82%92%E5%8F%96%E3%82%8A%E5%87%BA%E3%81%97%E3%81%A6%E5%89%8A%E9%99%A4%E3%81%99%E3%82%8B)
    - [引数を固定しない関数](#%E5%BC%95%E6%95%B0%E3%82%92%E5%9B%BA%E5%AE%9A%E3%81%97%E3%81%AA%E3%81%84%E9%96%A2%E6%95%B0)
      - [*argsを利用して、引数をタプルで受け取る](#args%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A6%E5%BC%95%E6%95%B0%E3%82%92%E3%82%BF%E3%83%97%E3%83%AB%E3%81%A7%E5%8F%97%E3%81%91%E5%8F%96%E3%82%8B)
      - [**kwargsを利用して、キーワード引数を辞書で受け取る](#kwargs%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A6%E3%82%AD%E3%83%BC%E3%83%AF%E3%83%BC%E3%83%89%E5%BC%95%E6%95%B0%E3%82%92%E8%BE%9E%E6%9B%B8%E3%81%A7%E5%8F%97%E3%81%91%E5%8F%96%E3%82%8B)
    - [osモジュールを利用して、カレントディレクトリの確認や移動を行う](#os%E3%83%A2%E3%82%B8%E3%83%A5%E3%83%BC%E3%83%AB%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A6%E3%82%AB%E3%83%AC%E3%83%B3%E3%83%88%E3%83%87%E3%82%A3%E3%83%AC%E3%82%AF%E3%83%88%E3%83%AA%E3%81%AE%E7%A2%BA%E8%AA%8D%E3%82%84%E7%A7%BB%E5%8B%95%E3%82%92%E8%A1%8C%E3%81%86)
    - [lambda式](#lambda%E5%BC%8F)
    - [ソート関数を作る](#%E3%82%BD%E3%83%BC%E3%83%88%E9%96%A2%E6%95%B0%E3%82%92%E4%BD%9C%E3%82%8B)
    - [map()](#map)
    - [イテレーターとは](#%E3%82%A4%E3%83%86%E3%83%AC%E3%83%BC%E3%82%BF%E3%83%BC%E3%81%A8%E3%81%AF)
    - [ジェネレーターとは](#%E3%82%B8%E3%82%A7%E3%83%8D%E3%83%AC%E3%83%BC%E3%82%BF%E3%83%BC%E3%81%A8%E3%81%AF)
    - [ジェネレーターに値を送る](#%E3%82%B8%E3%82%A7%E3%83%8D%E3%83%AC%E3%83%BC%E3%82%BF%E3%83%BC%E3%81%AB%E5%80%A4%E3%82%92%E9%80%81%E3%82%8B)
    - [初期化メソッド](#%E5%88%9D%E6%9C%9F%E5%8C%96%E3%83%A1%E3%82%BD%E3%83%83%E3%83%89)
    - [インスタンスを定義する](#%E3%82%A4%E3%83%B3%E3%82%B9%E3%82%BF%E3%83%B3%E3%82%B9%E3%82%92%E5%AE%9A%E7%BE%A9%E3%81%99%E3%82%8B)
    - [クラスメンバーとインスタンスメンバー](#%E3%82%AF%E3%83%A9%E3%82%B9%E3%83%A1%E3%83%B3%E3%83%90%E3%83%BC%E3%81%A8%E3%82%A4%E3%83%B3%E3%82%B9%E3%82%BF%E3%83%B3%E3%82%B9%E3%83%A1%E3%83%B3%E3%83%90%E3%83%BC)
    - [クラスメソッドを定義する](#%E3%82%AF%E3%83%A9%E3%82%B9%E3%83%A1%E3%82%BD%E3%83%83%E3%83%89%E3%82%92%E5%AE%9A%E7%BE%A9%E3%81%99%E3%82%8B)
    - [クラスの継承](#%E3%82%AF%E3%83%A9%E3%82%B9%E3%81%AE%E7%B6%99%E6%89%BF)
    - [スーパークラスの初期化メソッドをオーバーライドしないようにする](#%E3%82%B9%E3%83%BC%E3%83%91%E3%83%BC%E3%82%AF%E3%83%A9%E3%82%B9%E3%81%AE%E5%88%9D%E6%9C%9F%E5%8C%96%E3%83%A1%E3%82%BD%E3%83%83%E3%83%89%E3%82%92%E3%82%AA%E3%83%BC%E3%83%90%E3%83%BC%E3%83%A9%E3%82%A4%E3%83%89%E3%81%97%E3%81%AA%E3%81%84%E3%82%88%E3%81%86%E3%81%AB%E3%81%99%E3%82%8B)
    - [インスタンス変数をprivateにする](#%E3%82%A4%E3%83%B3%E3%82%B9%E3%82%BF%E3%83%B3%E3%82%B9%E5%A4%89%E6%95%B0%E3%82%92private%E3%81%AB%E3%81%99%E3%82%8B)
    - [プロパティを使ってprivateな変数にアクセスする](#%E3%83%97%E3%83%AD%E3%83%91%E3%83%86%E3%82%A3%E3%82%92%E4%BD%BF%E3%81%A3%E3%81%A6private%E3%81%AA%E5%A4%89%E6%95%B0%E3%81%AB%E3%82%A2%E3%82%AF%E3%82%BB%E3%82%B9%E3%81%99%E3%82%8B)
    - [ファイルを開く方法](#%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%82%92%E9%96%8B%E3%81%8F%E6%96%B9%E6%B3%95)
    - [折れ線グラフを描く](#%E6%8A%98%E3%82%8C%E7%B7%9A%E3%82%B0%E3%83%A9%E3%83%95%E3%82%92%E6%8F%8F%E3%81%8F)
    - [sinグラフを描く](#sin%E3%82%B0%E3%83%A9%E3%83%95%E3%82%92%E6%8F%8F%E3%81%8F)
    - [折れ線の種類やマーカを違う種類に設定し、凡例をつける](#%E6%8A%98%E3%82%8C%E7%B7%9A%E3%81%AE%E7%A8%AE%E9%A1%9E%E3%82%84%E3%83%9E%E3%83%BC%E3%82%AB%E3%82%92%E9%81%95%E3%81%86%E7%A8%AE%E9%A1%9E%E3%81%AB%E8%A8%AD%E5%AE%9A%E3%81%97%E5%87%A1%E4%BE%8B%E3%82%92%E3%81%A4%E3%81%91%E3%82%8B)
    - [棒グラフを作成する](#%E6%A3%92%E3%82%B0%E3%83%A9%E3%83%95%E3%82%92%E4%BD%9C%E6%88%90%E3%81%99%E3%82%8B)
    - [積み上げ棒グラフ](#%E7%A9%8D%E3%81%BF%E4%B8%8A%E3%81%92%E6%A3%92%E3%82%B0%E3%83%A9%E3%83%95)
    - [散布図を作成する](#%E6%95%A3%E5%B8%83%E5%9B%B3%E3%82%92%E4%BD%9C%E6%88%90%E3%81%99%E3%82%8B)
    - [サブプロットに描画する](#%E3%82%B5%E3%83%96%E3%83%97%E3%83%AD%E3%83%83%E3%83%88%E3%81%AB%E6%8F%8F%E7%94%BB%E3%81%99%E3%82%8B)
    - [軸のレンジを調整する](#%E8%BB%B8%E3%81%AE%E3%83%AC%E3%83%B3%E3%82%B8%E3%82%92%E8%AA%BF%E6%95%B4%E3%81%99%E3%82%8B)
      - [軸の最大値、最小値を指定する](#%E8%BB%B8%E3%81%AE%E6%9C%80%E5%A4%A7%E5%80%A4%E6%9C%80%E5%B0%8F%E5%80%A4%E3%82%92%E6%8C%87%E5%AE%9A%E3%81%99%E3%82%8B)
      - [Y軸を共有する](#y%E8%BB%B8%E3%82%92%E5%85%B1%E6%9C%89%E3%81%99%E3%82%8B)
    - [numpyの配列を作る](#numpy%E3%81%AE%E9%85%8D%E5%88%97%E3%82%92%E4%BD%9C%E3%82%8B)
    - [reshape()メソッドを利用して、1次元配列を多次元配列にする](#reshape%E3%83%A1%E3%82%BD%E3%83%83%E3%83%89%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A61%E6%AC%A1%E5%85%83%E9%85%8D%E5%88%97%E3%82%92%E5%A4%9A%E6%AC%A1%E5%85%83%E9%85%8D%E5%88%97%E3%81%AB%E3%81%99%E3%82%8B)
    - [ravel()またはflatten()を利用して、多次元配列を1次元配列に戻す](#ravel%E3%81%BE%E3%81%9F%E3%81%AFflatten%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A6%E5%A4%9A%E6%AC%A1%E5%85%83%E9%85%8D%E5%88%97%E3%82%921%E6%AC%A1%E5%85%83%E9%85%8D%E5%88%97%E3%81%AB%E6%88%BB%E3%81%99)
    - [構造を調べる](#%E6%A7%8B%E9%80%A0%E3%82%92%E8%AA%BF%E3%81%B9%E3%82%8B)
    - [要素を追加、挿入、削除する](#%E8%A6%81%E7%B4%A0%E3%82%92%E8%BF%BD%E5%8A%A0%E6%8C%BF%E5%85%A5%E5%89%8A%E9%99%A4%E3%81%99%E3%82%8B)
    - [transpose()関数または配列のTプロパティを利用し、転置する](#transpose%E9%96%A2%E6%95%B0%E3%81%BE%E3%81%9F%E3%81%AF%E9%85%8D%E5%88%97%E3%81%AEt%E3%83%97%E3%83%AD%E3%83%91%E3%83%86%E3%82%A3%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E8%BB%A2%E7%BD%AE%E3%81%99%E3%82%8B)
    - [多次元配列のスライス](#%E5%A4%9A%E6%AC%A1%E5%85%83%E9%85%8D%E5%88%97%E3%81%AE%E3%82%B9%E3%83%A9%E3%82%A4%E3%82%B9)
    - [降順にソート済みの配列を作る](#%E9%99%8D%E9%A0%86%E3%81%AB%E3%82%BD%E3%83%BC%E3%83%88%E6%B8%88%E3%81%BF%E3%81%AE%E9%85%8D%E5%88%97%E3%82%92%E4%BD%9C%E3%82%8B)
    - [numpy.linalg.norm()を利用して、ベクトルの長さを求める](#numpylinalgnorm%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A6%E3%83%99%E3%82%AF%E3%83%88%E3%83%AB%E3%81%AE%E9%95%B7%E3%81%95%E3%82%92%E6%B1%82%E3%82%81%E3%82%8B)
    - [mean()を利用して、平均値を求める](#mean%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A6%E5%B9%B3%E5%9D%87%E5%80%A4%E3%82%92%E6%B1%82%E3%82%81%E3%82%8B)
    - [標準偏差、偏差値](#%E6%A8%99%E6%BA%96%E5%81%8F%E5%B7%AE%E5%81%8F%E5%B7%AE%E5%80%A4)
    - [dot()を利用して行列の内積を求める](#dot%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A6%E8%A1%8C%E5%88%97%E3%81%AE%E5%86%85%E7%A9%8D%E3%82%92%E6%B1%82%E3%82%81%E3%82%8B)
    - [arrange()を利用して、連続番号の配列を作る](#arrange%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A6%E9%80%A3%E7%B6%9A%E7%95%AA%E5%8F%B7%E3%81%AE%E9%85%8D%E5%88%97%E3%82%92%E4%BD%9C%E3%82%8B)
    - [linespace()を利用して、等分割した値の配列を作る](#linespace%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A6%E7%AD%89%E5%88%86%E5%89%B2%E3%81%97%E3%81%9F%E5%80%A4%E3%81%AE%E9%85%8D%E5%88%97%E3%82%92%E4%BD%9C%E3%82%8B)
    - [eye()やidentity()を利用して、単位行列を作る](#eye%E3%82%84identity%E3%82%92%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A6%E5%8D%98%E4%BD%8D%E8%A1%8C%E5%88%97%E3%82%92%E4%BD%9C%E3%82%8B)
  - [Pythonではじめる機械学習 ―scikit-learnで学ぶ特徴量エンジニアリングと機械学習の基礎まとめ](#python%E3%81%A7%E3%81%AF%E3%81%98%E3%82%81%E3%82%8B%E6%A9%9F%E6%A2%B0%E5%AD%A6%E7%BF%92-%E2%80%95scikit-learn%E3%81%A7%E5%AD%A6%E3%81%B6%E7%89%B9%E5%BE%B4%E9%87%8F%E3%82%A8%E3%83%B3%E3%82%B8%E3%83%8B%E3%82%A2%E3%83%AA%E3%83%B3%E3%82%B0%E3%81%A8%E6%A9%9F%E6%A2%B0%E5%AD%A6%E7%BF%92%E3%81%AE%E5%9F%BA%E7%A4%8E%E3%81%BE%E3%81%A8%E3%82%81)
    - [sklearnでデータセットを訓練データとテストデータに分割する](#sklearn%E3%81%A7%E3%83%87%E3%83%BC%E3%82%BF%E3%82%BB%E3%83%83%E3%83%88%E3%82%92%E8%A8%93%E7%B7%B4%E3%83%87%E3%83%BC%E3%82%BF%E3%81%A8%E3%83%86%E3%82%B9%E3%83%88%E3%83%87%E3%83%BC%E3%82%BF%E3%81%AB%E5%88%86%E5%89%B2%E3%81%99%E3%82%8B)
    - [教師あり学習は分類と回帰に大別できる](#%E6%95%99%E5%B8%AB%E3%81%82%E3%82%8A%E5%AD%A6%E7%BF%92%E3%81%AF%E5%88%86%E9%A1%9E%E3%81%A8%E5%9B%9E%E5%B8%B0%E3%81%AB%E5%A4%A7%E5%88%A5%E3%81%A7%E3%81%8D%E3%82%8B)
    - [汎化とは](#%E6%B1%8E%E5%8C%96%E3%81%A8%E3%81%AF)
    - [過剰適合](#%E9%81%8E%E5%89%B0%E9%81%A9%E5%90%88)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# Python・機械学習まとめ

## [詳細！Python 3 入門ノート](https://www.amazon.co.jp/dp/B07171GVWK/ref=dp-kindle-redirect?_encoding=UTF8&btkr=1)まとめ

### ステートメントとは
- 命令文の単位をステートメントと呼ぶ。日本語の文の区切りは句読点だが、Pythonでのステートメントの区切りはセミコロン「;」である。
```py
a = 10; b = 20; ans = a + b
```
### ステートメントを途中で折り返したいとき
- ステートメントを折り返したいときは、改行したい行の最後で「\」を入力する
```py
ans = 1 + 2 + 3 \
+ 4 + 5....
```

### 値の区切り文字、改行を指定する

```py
a = 100
b = 200
c = 300
abc = a + b + c
print(a, b, c, sep = "、", end = "/以上")
# endの引数は行末文字、ここでは改行の代わりに出力する文字
print(abc)

"""実行結果
100、200、300/以上600
"""
```

### round
小数点以下を丸める関数。四捨五入とは違う。
例えば、2.5に近い整数は2または3だが、どちらも0.5の差なので、round(2.5)では偶数の2に丸める。
2.6は3に近いので3に丸める。

```py
>>> round(1.4)
1
>>> round(2.5)
2
>>> round(2.6)
3

# 小数点1位に丸める
>>> round(23.574, 1)
23.6
```

### ２進数、８進数、１６進数
pending
### 複素数
複素数の虚部にはjをつける

```py
>>> 1j * 1j
-1
```
複素数の実部はreal、虚部はimagで個別に取り出すことができる。
```py
>>> v = 3 + 2j
>>> v.real
3.0
>>> v.imag
2.0
```
複素数はcomplex(re, im)で作ることができる。
```py
>>> v = complex(3, 2)
>>> v
(3 + 2j)
```

### 数値演算子「//」
「a//b」で「aをbで割った商の整数値」
```py
>>> all = 350 # 全部の個数
>>> per = 12 # 1箱に12個入れる
>>> all // per # 完成する箱数
29
>>> all % per # 余る個数
2
```

### 複数行の文字列
クォートを３個続けて「"""~"""」というようにすると複数行の文字列を作ることができる。
```py
>>> poem = """ホトトギス
なきつる方をながむれば
ただ有明の月ぞ残れる"""

>>> print(poem)

"""実行結果
ホトトギス
なきつる方をながむれば
ただ有明の月ぞ残れる
"""
```

### []で文字列を取り出す
[]にはインデックス番号を指定する
```py
>>> id = "ab1cd9x"
>>> id[2]
'1'
>>> id[-1]
'x'
```

#### 部分文字列を抜き出す
抜き出す範囲は開始位置と終了位置で指定するが、開始位置〜（終了位置 - 1）の範囲になる。書式は以下の通り。
`文字列[開始位置:終了位置]`
```py
# 文字列[:]は文字列全体を返す
# 文字列[開始位置:]ならば開始位置から最後まで
# 文字列[：終了位置]ならば最初から終了位置の手前まで
>>> s = "The quick brown fox jumps."
>>> s[4:] # ５文字目から最後まで
'quick brown fox jumps'
>>> s[4:4+5] # 5文字目から５文字
'quick'
>>> s[:-7] # 先頭から、後ろから数えて７文字目の手前まで
'The quick brown fox'
```

#### ステップがある書式
`文字列[開始位置:終了位置:ステップ]`
```py
>>> num = "0123456789"
>>> n[::2] # 文字列から１つ飛ばして文字を取り出す
'02468'

>>> data = "abc0123456789"
>>> data[3::2] # ４文字目から１文字飛ばして取り出す
'02468'

>>> num = "0123456789"
>>> num[::-2] # 後ろから１文字飛ばし
'97531'

>>> s = "あいうえおかきくけこ"
>>> s[::-1] # 文字列を逆順にする
'こけくきかおえういあ'
```

### ビット演算子
pending

### 型を調べる
値の型はtype()で調べることができる。
```py
>>> type(1)
<class 'int'>
```

### リテラルとリファレンス
リテラルとは、10、20、"abc"など、コードに値を直接書いたもの。
これに対しリファレンスは値が記録されているアドレスへの参照。

### mathモジュールに含まれる関数

```py
>>> import math
>>> math.ceil(15.2) # ceil関数は小数点以下を切り上げる関数
16
>>> math.floor(15.2) # 切り捨ての関数
15

>>> math.pi # 円周率
3.1415....
>>> math.degrees(math.pi/4) # ラジアンを度に換算
45.0

# floorは小数点以下を切り捨てするので、小数点第２位で切り捨てたい場合は
# 100倍して切り捨てた後に100で割る
>>> kyori = 20
>>> kakudo = math.radians(32) # ラジアンに換算する
>>> takasa = kyori * math.tan(kakudo)
>>> takasa = math.floor(takasa * 100)/100
print(str(takasa) + "m")
12.49m
```

### 関数を指定して読み込む

```py
>>> from random import randint # randint()は整数の乱数を生成する関数
>>> randint(1, 6) # 1~6の乱数を生成
5
4
1
5
.
.

```

### 大文字小文字の変換

```py
>>> s = "AppleとGoogle"
>>> s.upper() # upperメソッドは全て大文字化するメソッド
'APPLEとGOOGLE'
>>> s.lower() # lowerメソッドは全て小文字化するメソッド
'appleとgoogle'
>>> s.swapcase() # swapcaseは大文字と小文字を入れ替えるメソッド
'aPPLEとgOOGLE'
>>> s = "may the force be with you"
>>> s.capitalize() # capitalizeは文字列の１文字目だけを大文字にし以降を小文字にするメソッド
'May the force be with you'
>>> s.title() # titleは各単語の１文字目を大文字にし、単語の２文字目以降を小文字にするメソッド
'May The Force Be With You'
```

### 文字列を検索する
#### countメソッド
count()は文字列を検索して、引数で指定した文字列が何個含まれているかを返す。
```py
>>> s = "apple pie"
>>> s.count("p") # "p"の個数を数える
3
```
検索範囲を指定するやり方もあり`count(文字列, 開始位置, 終了位置)`とすると、開始位置から終了位置の手前までを検索する

```py
>>> s = "apple pie"
>>> s.count("p", 0, 4)
2
```

#### findメソッド
find()は文字が見つかった最初の位置を返し、見つからなかった場合は-1を返す。
`find(文字列, 開始位置, 終了位置)`

```py
>>> s = "apple pie"
>>> s.find('e')
4
>>> s.find("x")
-1
>>> s.rfind("e") # rfindメソッドは最後に見つかった位置を返す。
8
```

### 文字列を置換する
`replace(検索文字列, 置換文字列, 個数)`

```py
>>> s = "employee"
>>> s.replace("e", "x")
'xmployxx'
>>> s.replace("e", "x", 2) # 置換する個数を指定した
'xmployxe'
```
### 余分な文字を取り除く
strip()は文字列の先頭と末尾にある余分な文字を取り除き、rstrip()は末尾にある余分な文字を取り除く

```py
>>> t = "  hello  \n"
>>> t.strip()
'hello'
>>> t = "abc...."
>>> t.rstrip(".") # 取り除く文字を指定する
'abc'
```

### 文字列に値を埋め込む
文字列に埋め込みたい値をformat()の引数に指定すると、その値が順に文字列の中の置換フィールドである{}の位置に入る。
```py
>>> s = "チューリップは{}と{}と{}でした"
>>> s.format("赤", "青", "黄色")
'チューリップは赤と青と黄色でした'
```

```py
>>> name = "高橋"
>>> age = 23
>>> point = 102.5
>>> s = "{}選手, 年齢{}、得点{}でした。"
>>> text = s.format(name, age, point)
>>> print(text)
高橋選手、年齢23、得点102.5でした。

# 上のコードをf"{値}"の書式を使って書き直す。
>>> name = "高橋"
>>> age = 23
>>> point = 102.5
>>> text = f"{name}選手、年齢{age}、得点{point}でした。"
>>> print(text)
高橋選手、年齢23、得点102.5でした。
```
### 値の書式設定
`{値:書式}`
```py
# 数値を位取りして埋め込む
>>> tokyo = 123456000
>>> kyoto = 53900
>>> print(f"東京{tokyo:,}、京都{kyoto:,}") # 3桁位取り
東京123,456,000、京都53,900

# formatを使用する場合
>>> s = "東京{:,}、京都{:,}"
>>> s.format(tokyo, kyoto)
'東京123,456,000、京都53,900'

# 小数点以下の桁数指定
# 浮動小数点は.桁fで小数点以下の桁数も指定できる
>>> length = 25.34
>>> thickness = 5.62
>>> text = f"長さ{length:.1f}cm、厚み{thickness:.0f}mm"
# lengthは小数点以下1位まで、thicknessは小数点以下を表示しない
>>> print(text)
長さ25.3cm、厚み6mm

# formatを使う場合
>>> s = "長さ{:.1f}cm、厚み{:.0f}mm"
>>> s.format(length, thickness)

# 位取りと小数点以下の桁数指定を行いたい場合
>>> num = 2345.032
>>> print(f"{num:,.2f}")
2,345.03
```

### 値の位置揃え
位置揃えは、左詰「<」、中央揃え「^」、右詰「>」で指定する。
```py
>>> num1 = 123.4
>>> num2 = 56.9
>>> num3 = 3040.1
>>> print(f"{num1:>10.1f}")
# 全体が10文字の幅で小数点１位まで
      123.4
```

### if文

```py
# randomモジュールのrandint関数を読み込む
from random import randint
size = randint(5, 20) # 5~20の乱数
weight = randint(20, 40) # 20~40の乱数
if (size >= 10) and (weight >= 25):
      result = "合格"
else:
      result = "不合格"

text = f"サイズ{size}、重量{weight}:{result}"
print(text)
```

### Falseとみなされる値
- False
- None
- 数値の 0、0.0、0j
- 空の値 ""、()、[]、{}

```py
from random import randint
num = randint(0, 100)
# 奇数か偶数かを判定する
if num % 2: # 2で割り切れる偶数は余り０でFalse、奇数は余り１でTrue.
      result = "奇数"
else:
      result = "偶数"
print(num, result)
```

### Pythonでの三項演算子の代わり
```py
from random import randint
a = randint(0, 100) 
b = randint(0, 100)
# 大きい方の値を代入する
bigger = a if a>b else b # a>bがtrueならばa、Falseならばbを代入
text = f"{a}と{b}では{bigger}が大きい"
print(text)
```

### while文
```py
from random import randint
tickets = 5
point = 0
fmt = "{:>3}" # 3桁右詰
while tickets > 0:
      v = randint(1, 20)
      print(fmt.format(v))
      point += v
      tickets -= 1
print("-" * 3)
print(fmt.format(point))
```

### break
```py
# ３回間違えるか、"q"と入力されるまで出題を繰り返す
from random import randint
miss = 0 # 間違えた数
correct = 0 # 正解数
print("問題！３回間違えたら終了。qで止める")
while miss < 3:
      a = randint(1, 100)
      b = randint(1, 100)
      ans = a + b
      # 問題を出題し、キーボードからの入力待ちにする
      question = f"{a}+{b}は?"
      value = input(question)
      # qと入力されたら中断する
      if value == "q":
            break # ブレイクする
      # 解答が正解かどうか判定する
      if value == str(ans):
            correct += 1
            print("正解です！")
      else:
            miss += 1 # 間違いをカウントアップする
            print("間違い！", "x" * miss) # 間違いの数だけXを表示する
print("-" * 20)
print("正解:", correct)
print("間違い：", miss)
```

### continue
```py
from random import randint
numbers = []
# numbersの数が10個になるまで繰り返す
while len(numbers) < 10:
      n = randint(0, 100)
      if n in numbers:
      # nがnumbersに含まれていたらスキップする
            continue # すでに含まれている値は追加せずに処理をスキップする
      # numbersにnを追加する
      numbers.append(n)
print(numbers)
```

### while~else文
繰り返しが終了した時点でelseブロックが実行される。途中でbreakされた場合はelseブロックは実行されない。

```py
from random import randint
numbers = []
# numbersの数が10個になるまで繰り返す
while len(numbers) < 10:
      n = randint(-10, 90)
      if n < 0:
            print('中断されました')
            break # elseブロックを実行せずに終了する
      if n in numbers:
      # nがnumbersに含まれていたらスキップする
            continue # すでに含まれている値は追加せずに処理をスキップする
      # numbersにnを追加する
      numbers.append(n)
else:
     print(numbers)
```

### range関数
`range(開始値, 終了値, ステップ)`
```py
for i in range(5, 10):
      print(i)
>>>5
>>>.
>>>.
>>>9 # 10ではないことに注意
```
```py
# ４行３列の点の座標を求める
for i in range(4): # 4行
      print() # 改行
      for j in range(3): # 3行
            x = j * 2
            y = i * 3
            print(f"{x}, {y}", end="")
print() # 最後の改行
```

### for文でのbreak

```py
numlist = [3, 4.2, 10, "x", 1, 9]
sum = 0
for num in numlist:
      # numが数値でない時breakする
      if not isinstance(num, (int, float)): # intかfloatでない時
            print(num, "数値ではありません")
            break
      sum += num
      print(num, "/", sum)

```

### for in ~ else
繰り返しが終了した時点でelseブロックが実行される。途中でbreakされた場合はelseブロックは実行されない。

```py
numlist = [3, 4.2, 10, "x", 1, 9]
sum = 0
for num in numlist:
      # numが数値でない時breakする
      if not isinstance(num, (int, float)): # intかfloatでない時
            print(num, "数値ではありません")
            break
      sum += num
else:
      print("合計", sum)
```

### 例外処理
- エラーが発生する可能性のあるステートメントをtryブロックで実行する
- エラーが起こった場合、エラーを通知するの例外オブジェクトをexceptブロックで受け止めて例外処理を実行する。
- エラーが発生しなければexceptブロックは実行させない
- exceptブロックは例外ハンドラとも呼ばれる。

```py
try:
      例外が発生する可能性がある処理
except:
      例外を受けて実行する処理
```

```py
while True:
      num = input("何個ですか?(qで終了)")
      if num == "q":
            print("終了しました")
            break
      try:
            price = 120 * int(num)
            print("金額", price)
      except:
            print("エラー")
```

#### try + except + finally
- finallyは例外が発生しても発生しなくてもtry文を抜ける前に必ず実行するブロック
- finallyブロックではtryで実行した処理の後始末を行う

```py
try:
      例外が発生する可能性がある処理
except:
      例外を受けて実行する処理
finally:
      try文を抜ける前に必ず実行する処理
```

#### 例外オブジェクトによって処理を振り分ける

```py
try:
      例外が発生する可能性がある処理
except 例外１:
      例外１に対応する処理
except 例外２:
      例外２に対応する処理
except :
      例外１、２のどちらでもない例外の処理
```

```py
# 1つのexceptブロックに対して複数の例外をタプルで割り当てる
try:
      例外が発生する可能性がある処理
except (例外１,例外２):
      例外１、例外２に対応する処理
except (例外３,例外４):
      例外３、例外４に対応する処理
except :
      例外１〜４ではない例外の処理
```

```py
# 型変換の例外はValueError
# ゼロの割り算の例外はZeroDivisionError
sum = 7600
while True:
      num = input("何人ですか?(qで終了)")
      if num == "q":
            print("終了しました")
            break
      # 例外を振り分けて例外処理を行う
      try:
            price = round(sum / int(num))
            if price < 0:
                  continue
            print("一人当たりの金額", price)
      except ValueError:
            print("数値を入れてください")
      except ZeroDivisionError:
            print("0以外の数値を入れてください")
```

#### try + except + except + else + finally
elseは例外が発生しなかった時に実行される。

```py
try:
      例外が発生する可能性がある処理
except 例外１:
      例外１に対応する処理
except 例外２:
      例外２に対応する処理
else:
      例外が発生しなかった時に実行する処理
finally:
      try文を抜ける前に必ず実行する処理
```

#### 例外情報を調べる except as
asキーワードで名前を指定すると、例外をその名前の変数に一時的に保管できる
```py
try:
      実行を試すステートメント
except 例外１ as 名前１:
      例外１に対応するステートメント
except 例外2 as 名前2:
      例外2に対応するステートメント
```
以下のコードでは例外をEXceptionで受け取り、その例外オブジェクトを変数errorに代入している。そしてerrorを出力することで、どんなエラーなのかをエラー情報として出力している。
```py
sum = 7600
while True:
      num = input('何人ですか？（qで終了）')
      if num == 'q':
            print("終了しました。")
            break
      # 例外を処理する
      try:
            price = round(sum / int(num))
      except Exception as error: # 例外オブジェクトをerrorで参照できるようにする
            print('エラー ')
            print(error) # エラー情報を出力する
      else: # 例外が発生しなかった場合はelseブロックが実行される
            if price < 0:
                  continue
            print("一人当たりの金額", price)

```

### リスト

#### list()
他の型の値をリストに変換できる

```py
>>> evenlist = list(range(0, 10, 2))
>>> evenlist
#=> [0, 2, 4, 6, 8]

>>> week = list("日月火水木金土")
>>> week
#=> ['日', '月', '火', '水', '木', '金', '土']
```

#### リストのインデックスエラーを回避する
- リストに存在しないリストを参照するとインデックスエラーになる。
- インデックスエラーを回避するには、リストの長さ（要素の個数）を`len()`で調べる。

```py
pos = int(input("取り出す位置："))
colors = ["blue", "red", "green", "yellow"]
length = len(colors)
if -length <= pos < length:
      item = colors[pos]
      print(item)
else:
      print("エラーになりました。")
```

#### リストの末尾に要素を追加する
`append(値)`
```py
>>> data = []
>>> data.append(10)
>>> data.append(20)
>>> data
[10, 20]
```

#### 指定の位置に要素を挿入する
- `insert()`を使って挿入位置をインデックス番号で指定する。
- 新しい要素が挿入されると元の要素は後ろにずれる。
- `insert(挿入位置, 値)`

```py
>>> data = ["a", "b", "c", "d"]
>>> data = insert(3, "new")
>>> data
["a", "b", "c", "new", "d"]
```

### リストの要素を削除する
- `pop()`メソッドを使う。
- `pop()`は削除と同時に削除した要素を返すので、箱から物を取り出すようにリストから要素を抜き取りたい時に使う
- `pop()`とするとリストの最後の要素を削除する
- `pop(抜き取る位置)`でインデックス番号を指定すると、特定の要素を削除できる。

```py
# fruits.pop()を実行して値を抜き取ってdessertに入れる
>>> fruits = ["apple", "lemon", "banana", "orange"]
>>> dessert = fruits.pop()
>>> dessert
"orange"
>>> fruits
["apple", "lemon", "banana"]

# fruits.pop(0)で先頭の要素を抜き出してdessert2に入れる
>>> dessert2 = fruits.pop(0)
>>> dessert2
"apple"
>>> fruits
["lemon", "banana"]
```

### 指定の値を削除する
- `remove()`で値を指定して削除する
- `remove()`で削除しようとした値がリストに含まれていない場合はエラーになるので、in演算子でチェックする
```py
colors = ["blue", "red", "yellow", "red", "green"]
target = "yellow"
# 削除する値が含まれているならば削除する
if target in colors:
      colors.remove(target)


# 上のifをwhileに変えるだけで削除対象の値がリストに残っている限り削除するようにできる。
```

### split
```py
# 事前に空白を取り除いてから分割する
>>> colors = "red,blue,   green,  white , black"
>>> colors = colors.replace(" ", "") # 空白を取り除く
>>> color_list = colors.split(",") # 感まで分割する
>>> color_list
['red', 'blue', 'green', 'white', 'black']

# splitで作ったリストの先頭から３要素をスライスしたリストを作る
>>> result = "10", "11", "12", "13", "14"
>>> result_list = result.split(",", 3)
>>> result_list
["10", "11", "12", "13,14"]
>>> top3 = result_list[:3]
>>> top3
["10", "11", "12"]
```

### リストを連結する
- `+=`を使う
- `extend()`を使う
```py
>>> data = [1, 3, 5]
>>> newdata = [2, 4, 6]
>>> data.extend(newdata)
>>> data
[1, 3, 5, 2, 4, 6]
# data += newdataとしても同じ
```

### リストのスライス
`リスト[開始位置:終了位置]`
- 抜き出す範囲は開始位置~(終了位置-1)

### 値やオブジェクト比較
- 値が同じかどうかは\==演算子を使い、オブジェクトが同一かどうかは`is`、`is not`の演算子を使う。

```py
>>> list_a = [1, 2, 3]
>>> list_b = list_a
>>> list_c = [1, 2, 3]
>>> list_a is list_b
True
>>> list_a is list_c
False
>>> list_a is not list_c
True
```

### 参照
- 同じオブジェクトを参照している変数の一つに別の変数や値を代入して場合、変数に入れている参照を書き換えたことになるので、同じオブジェクトを参照している変数とは無関係になる。
- 以下の例ではlist2にlist1を代入して同じリストを参照している状態を作っている。しかし、その後でlist1に別のリストを代入している。そうした場合、最初にlist1に代入された参照を記録しているので、list2の値は代入された`[10, 20, 30]`から変化しない。
```py
>>> list1 = [10, 20, 30]
>>> list2 = list1
>>> list1 = [11, 22, 33]
>>> list2
[10, 20, 30]
```

### リストの複製
- `copy()`を使用する
- `[:]`を使用する
- `list()`を使用する

```py
>>> list_mother = [1, 2, 3, 4]
>>> list_work = list_mother.copy()
>>> list_work
[1, 2, 3, 4]

>>> list_work2 = list_mother[:]
>>> list_work2
[1, 2, 3, 4]

>>> list_work3 = list(list_mother)
>>> list_work3
[1, 2, 3, 4]
```

### リストの要素をソートする

```py
>>> numbers = [9, 4, 5, 8, 3]

# 昇順にソートする
>>> numbers.sort()
>>> numbers # 元のリストが変更される
[3, 4, 5, 8, 9]

# 降順にソートする
>>> numbers.sort(reverse = True)
>>> numbers
[9, 8, 5, 4, 3]
```

### ソートした新しいリストを作る
- `sort()`は元のリストの値を直接並び替えるが、`sorted()`は元になっているリストは変更せずにソート後の新しいリストを作る

```py
>>> numbers = [42, 35, 56, 21, 3]
>>> numbers_ascend = sorted(numbers)
>>> numbers_ascend
[3, 21, 35, 42, 56] # ソート済みの新しいリストが作成される
>>> numbers
[42, 35, 56, 21, 3] # 元のリストは変化しない
```

### 単純にリストの要素の並び順を逆順にしたい場合
- `reverse()`を使う
```py
>>> numbers = [42, 35, 56, 21, 3]
>>> numbers.reverse()
>>> numbers # 元のリストが変更される
[3, 21, 56, 35, 42]
```

### リストの要素をランダムにならべかえる
- randomモジュールの`shuffle()`を利用する
```py
# 0~9が順に入ったリストnumbers()を作成し、
# random.shuffle()を使って数値がランダムなリストに変更する
>>> import random
>>> numbers = list(range(10))
>>> random.shuffle(numbers)
>>> numbers
[2, 8, 3, 1, 9, 7, 4, 5, 0]
```

### ソートで使う比較関数を指定する
- 比較関数を指定する際はkeyオプションを使用する
```py
# 文字列の長さでソートする
>>> words = ["chest", "wind", "holiday", "knight", "silence", "hot"]
>>> words.sort(key = len)

# 大文字小文字を区別せずソートする
>>> words = ["peach", "ver3", "Python", "Pokemon", "ver2"]
>>> new_words = sorted(words, key = str.lower) # 小文字でソートして比較する
```

### for文でカウンタをつけて表示する
- `enumerate()`を利用する
- 以下のコードではiにカウンタの値が入り、whoにnamesから取り出した要素が入る。

```py
names = ["鈴木", "田中", "栗林", "山岡"]
for i, who in enumerate(names, 1): # １からカウントアップする
      print(f"{i}:{who}さん")
```

### for文で複数のリストを対象にする

```py
name1 = ["鈴木", "田中", "赤尾", "佐々木", "高田"]
name2 = ["星奈", "優美", "恵子", "薫花", "幸恵"]
longname = []
for n1, n2 in zip(name1, name2):
      longname.append(n1+n2)
```

### リスト内包表記
- イテラブル：値に含まれている要素を順に１個ずつ要素を取り出すことができるオブジェクトのこと
- リストや文字列、辞書などがイテラブル。
`[式 for 変数 in イテラブル]`

```py
>>> nums = [1, 2, 3, 4, 5, 6]
# numsから取り出した値を２倍にしたリストを作る
>>> nums_double = [num*2 for num in nums]
>>> nums_double
[2, 4, 6, 8, 10, 12]

# 数値を整数に切り捨てたリストを作る
>>> import math
>>> num_list = [1.5, 2.6, 3.3, 4.3]
>>> result = [math.floor(num) for num in num_list]
>>> result
[1, 2, 3, 4]

# 文字列からリストを作る
>>> group_list = [f"{str}組" for str in "ABC"]
>>> group_list
["A組", "B組", "C組"]

# zip()を使って2つのリストを連結する
>>> name1 = ["鈴木", "田中", "赤尾"]
>>> name2 = ["星奈", "優美", "恵子"]
>>> longname = [n1 + n2 for n1, n2 in zip(name1, name2)]
>>> longname
["鈴木星奈", "田中優美", "赤尾恵子"]
```

### 条件式付きのリスト内包表記
`[式 for 変数 in イテラブル if 条件式]`

```py
# １以上２未満の数値だけ取り出したリストを作る
>>> numbers = [2.1, 0.2, 1.4, 3.1, 1.6]
>>> result = [num for num in numbers if 1<=num<2]
>>> result
[1.4, 1.6]

# 数値以外の値を取り除く
numbers = [2.1, 4, "", 2.2, "1", 3]
# isinstance(num, (int, float))は、numがintかfloatの時Trueになる
>>> numbers = [num for num in numbers if isinstance(num, (int, float))]
>>> numbers
[2.1, 4, 2.2, 3]
```

### indexメソッド
- 見つかった位置を返すメソッド
- 見つからなかったときは例外のValueErrorが発生する

```py
# 入力されたidが見つかったら登録順番、見つからなかったメッセージを出す
id_list = ["a2345", "a1236", "b7656", "f0987"]
while True:
      id = input("idを入力してください(qで終了):")
      if id == "q":
            print('終了しました')
            break
      # 例外処理に組み込んで検索する
      try:
            pos = id_list.index(id)
            print(str(pos + 1) + "番目のメンバーです。")
      except:
            print('メンバーではありません')
```

### 個数を調べる
- `count()`を利用する
```py
>>> numbers = [1, 3, 4, 5, 5, 15, 12, 57]
>>> numbers.count(2) # 2が何個あるか数える
0
>>> numbers.count(4)
1
```

```py
# resultに含まれている1が半数以上ならば「合格」にする
result = [1, 1, 0, 0, 1, 0, 1, 1]
half = len(result) / 2
point = result.count(1)
if point >= half:
      print('合格')
else:
      print('不合格')
```

### リストから要素をランダムに取り出したい場合
- secretsモジュールのchoice()を利用する
```py
>>> import secrets
>>> fruits = ["apple", "orange", "banana", "peach"]
>>> dessert = secrets.choice(fruits)
>>> dessert
"apple"
```

### tuple()を使って文字列を分解してタプルにする

```py
>>> week = tuple("日月火水木金土")
>>> week
("日","月", "火", "水", "木", "金", "土")
```

### セット
- 1つのセットの中に同じ値の要素を重複して入れることができない
- セットの要素には順序がない

```py
>>> num2set = set(range(0, 10, 2)) # 0~9の2の倍数のセット
>>> num2set
{0, 2, 4, 6, 8}
```

### セットに要素を追加する

```py
>>> fruits = set()
>>> fruits.add("apple")
>>> fruits.add("orange")
>>> fruits
{'apple', 'orange'}
```

### セットから要素を削除する

```py
>>> fruits
{'apple', 'orange', 'banana', 'peach'}
>>> fruits.remove("banana")
>>> fruits
{'apple', 'orange', 'peach'}

# remove()で存在しない要素を削除しようとするとエラーになるが
# discard()を使うとエラーにならず操作が無視される。
```

### frozenset型のセット
- frozenset型は後から追加や削除などの変更ができない。

```py
>>> dataset = frozenset(["a", "b", "c"])
>>> dataset
frozenset({"a", "b", "c"})
>>> type(dataset)
<class 'frozenset'>
```

### セットの集合演算

### セットの和集合

```py
# |を使った和集合。セット同士
>>> a = {"リンゴ", "みかん", "桃", "いちご"}
>>> b = {"いちご", "スイカ", "みかん", "バナナ"}
>>> c = {"いちご", "リンゴ"}
>>> d = a | b | c
>>> d
{"リンゴ", "みかん", "桃", "いちご", "スイカ", "バナナ"}


# union()を使った和集合。セット以外のイテラブルとの和集合も可能
>>> set1 = {1, 2, 3}
>>> list1 = [2, 4, 6, 8]
>>> list2 = [3, 6, 9]
>>> data = set1.union(list1, list2)
>>> data
{1, 2, 3, 4, 6, 8, 9}
```

### セットの積集合

```py
# &を使った積集合
>>> a = {"リンゴ", "みかん", "桃", "いちご"}
>>> b = {"いちご", "スイカ", "みかん", "バナナ"}
>>> c = {"いちご", "リンゴ"}
>>> d = a & b & c
>>> d
{"いちご"} # 3つの集合で共通している要素が入っている
```
```py
# intersection()を使った積集合
>>> a = {"リンゴ", "みかん", "桃", "いちご"}
>>> b = {"いちご", "スイカ", "みかん", "バナナ"}
>>> c = {"いちご", "リンゴ"}
>>> d = a.intersection(b, c)
>>> d
{"いちご"}
```

### セットの差集合
```py
# -を使った差集合
>>> a = {"リンゴ", "みかん", "桃", "いちご"}
>>> b = {"いちご", "スイカ", "みかん", "バナナ"}
>>> c = a - b
>>> c
{'リンゴ', '桃'}
```
```py
# difference()を使った差集合
>>> a = {"リンゴ", "みかん", "桃", "いちご"}
>>> b = {"いちご", "スイカ", "みかん", "バナナ"}
>>> c = a.difference(b)
>>> c
{'リンゴ', '桃'}
```

### セットの対称差集合
- aセットとbセットのどちらか一方のみに含まれている要素を取り出したcセットを作る
```py
# ^を使った対称差集合
>>> a = {"リンゴ", "みかん", "桃", "いちご"}
>>> b = {"いちご", "スイカ", "みかん", "バナナ"}
>>> c = a ^ b
>>> c
{"リンゴ", "スイカ", "桃", "バナナ"} # 片方だけに含まれている要素の集合が作られる
```
```py
# symmetric_difference()を使った差集合
>>> a = {"リンゴ", "みかん", "桃", "いちご"}
>>> b = {"いちご", "スイカ", "みかん", "バナナ"}
>>> c = a.symmetric_difference(b)
>>> c
{"リンゴ", "スイカ", "桃", "バナナ"} 
```

### 集合演算結果でセットの内容を更新する

```py
# セットの値を和集合で更新する
>>> data = {"red", "blue"}
>>> data2 = {"blue", "yellow"}
>>> data3 = {"blue", "green"}
>>> data.update(data2, data3)
>>> data
{"red", "blue", "yellow", "green"}

# |=演算子を使って和集合の代入をする
>>> data |= data2
>>> data |= data3
>>> data
{"red", "blue", "yellow", "green"}



# セットの値を積集合で更新する
>>> data = {"red", "blue", "green", "yellow"}
>>> data2 = {"blue", "black", "yellow"}
>>> data.intersection_update(data2)
>>> data
{'blue', 'yellow'}

# &=演算子を使って積集合の代入をする
>>> data = {"red", "blue", "green", "yellow"}
>>> data2 = {"blue", "black", "yellow"}
>>> data &= data2
>>> data
{'blue', 'yellow'}



# セットの値を差集合で更新する
>>> data = {"red", "blue", "green", "yellow"}
>>> data2 = {"blue", "black", "yellow"}
>>> data.difference_update(data2)
>>> data
{'red', 'green'}

# -=演算子を使って差集合で更新する
>>> data = {"red", "blue", "green", "yellow"}
>>> data2 = {"blue", "black", "yellow"}
>>> data -= data2
>>> data
{'red', 'green'}



# セットの値を対称差集合で更新する
>>> data = {"red", "blue", "green", "yellow"}
>>> data2 = {"blue", "black", "yellow"}
>>> data.symmetric_difference_update(data2)
>>> data
{'red', 'green', 'black'}

# ^=演算子を使って対称差集合で更新する
>>> data = {"red", "blue", "green", "yellow"}
>>> data2 = {"blue", "black", "yellow"}
>>> data ^= data2
>>> data
{'red', 'green', 'black'}
```

### セット同士に共通要素があるかどうかを判定する
- isdisjoint(other)で判定する。共通要素がないときにTrue。共通要素があるとFalseになる

```py
>>> a = {"earth", "wind", "fire"}
>>> b = {"sky", "sea"}
>>> c = {"fire", "water"}
>>> a.isdisjoint(b) # aとbには共通要素がない
True
>>> a.isdisjoint(c) # aとcにはどちらも'fire'がある
False
```

### セットの包含関係を調べる
- aセットの要素が全てbセットに含まれているとき、aセットはbセットのサブセット、bセットはaセットのスーパーセットであるという

```py
# aセットがbセットのサブセットであるかどうかはa.issubset(b), a<b, a<=bで判定できる
>>> a = {"blue", "red"}
>>> b = {"blue", "green", "red", "pink", "white"}
>>> a.issubset(b) # aはbのサブセットである
True

# 一方、スーパーセットはa.issuperset(b), a>b, a>=bで判定できる
>>> a = {1999, 2011, 2013, 2014, 2016, 2017}
>>> b = {2011, 2013, 2014}
>>> a.issuperset(b)
True
```

### タプル（キー, 値）のリストから辞書を作る
- （キー, 値）のようにキーと値をペアにしてタプルを作り、これをリストにしてdict()の引数として渡す
```py
>>> data = dict([("yellow", 3), ("blue", 6), ("green", 5)])
>>> data
{'yellow': 3, 'blue': 6, 'green': 5}
```

### zip()を利用し、キーと値のリストを合わせて辞書にする
- zip()を利用するとキーのリストと値のリストを合わせて、（キー, 値）のタプルのリストを作ることができる。
```py
>>> keys = ["yellow", "blue", "green"]
>>> values = [3, 6, 5]
>>> data = dict(zip(keys, values))
>>> data
{'yellow': 3, 'blue': 6, 'green': 5}
```

### キーワード引数を利用して辞書を作る
```py
>>> data = dict(yellow = 3, blue = 6, green = 5)
>>> data
{'yellow': 3, 'blue': 6, 'green': 5}
```

### 初期値で辞書を作る
`dict.fromkeys(イテレータ, 初期値)`
```py
>>> stock = dict.fromkeys(["S", "M", "L"], 0)
>>> stock
{'S': 0, 'M': 0, 'L': 0}
```

### setdefault()を利用して、キーがあればそのまま、なければ追加する
- setdefault()はキーで指定した要素が存在しない時に要素を追加する。指定したキーがすでに存在しているときは値を置き換えない。
```py
>>> data = {"yellow": 3, "blue": 6, "green": 5}
>>> data.setdefalut("blue", 10) # "blue"キーがあるので何も変更しない
6
>>> data.setdefalut("white", 10) # "white"キーがあるので要素を追加する
10
>>> data
{'yellow': 3, 'blue': 6, 'green': 5, "white": 10}
```

### update()を利用して他の辞書を更新する
```py
>>> data = {"a": 10, "b": 20, "c": 30}    # 元の辞書
>>> newdata = {"a": 15, "d": 99}    # 更新用の辞書
>>> data.update(newdata)    # dataを更新する
>>> data
{"a": 15, "b": 20, "c": 30, "d": 99} 
```

### delを利用して、指定のキーの要素を削除する
```py
>>> fruit = ["apple": 7, "orange": 5, "mango": 3]
>>> del fruit["mango"]
>>> fruit
{'apple': 7, 'orange': 5}
```

### 辞書内包表記
```py
>>> from random import randint
>>> keys = ["green", "red", "blue", "yellow"]
>>> data = {key: randint(1, 100) for key in keys}
>>> data
{"green": 27, "red": 56, "blue": 24, "yellow": 94}
```

### dict.fromkeys()を利用して、同じ構造の辞書を作る
```py
>>> fruit = {"apple": 7, "orange": 5, "mango": 3, "peach": 6}
>>> fruit2 = dict.fromkeys(fruit, 0)
>>> fruit2
{"apple": 0, "orange": 0, "mango": 0, "peach": 0}
```

### pop()を利用して、指定したキーの値を取り出して、削除する
- pop()は指定したキーを取り出し、その要素を辞書から削除する
- 指定したキーが存在しない場合はKeyErrorとなる
```py
fruit = {"apple": 7, "orange": 5, "peach": 6}
while fruit: # fruitが空でなければ繰り返す
      key = input("どのフルーツを取り出しますか?(qで終了):")
      if key == "" :
            continue
      elif key == "q" :
            print("終了しました")
            break
      try :
            value = fruit.pop(key) # keyの値を取り出して削除
            print(f"{key}は{value}個") # 取り出したキーと値を表示
      except Keyerror : # 入力されたキーが辞書になかったらメッセージを表示
            print(f"{key}はありません")
      except Exception as error :
            print(error)
            break
else : # whileループの終了後に実行
      print("もう空っぽです")
```

### 引数を固定しない関数

#### *argsを利用して、引数をタプルで受け取る
- `*args`のようにすると、引数argsには渡された値がタプルにまとめて入る
```py
def route(start, end, *args):
      route_list = [start] # スタート地点
      route_list += list(args) # 経由地点
      route_list += [end] # ゴール地点
      # リストの要素を→で連結した文字列を作る
      route_str = "→".join(route_list)
      print(route_str)

# route()を試す
start = "東京"
end = "宮崎"
route(start, end, "神戸", "長崎", "熊本")

"""実行結果
東京→神戸→長崎→熊本→宮崎
"""
```

#### **kwargsを利用して、キーワード引数を辞書で受け取る
- 複数のキーワード引数をまとめて辞書に変換して受け取る
```py
def entry(name, gender, **kwargs):
      data = {"name" : name, "gender" : gender}     # 必須の引数の辞書
      data.update(kwargs)
      print(data)

entry(name="大山坂道", gender="男性", age=27, course="E")

"""実行結果
{ 'name': "大山坂道", 'gender': "男性", 'age': 27, 'course' "E" }
"""
```

### osモジュールを利用して、カレントディレクトリの確認や移動を行う
- osモジュールを使うとPythonインタプリタ内でディレクトの移動ができる
```py
>>> import os
>>> os.getcwd()    # カレントディレクトリを確認する

>>> os.chdir("./Section10-3")    # 現在のディレクトリにあるSection10-3フォルダに移動する
>>> os.getcwd()

>>> os.chdir("../Section10-4")    # 同じ階層のSection10-4フォルダに移動する
>>> os.getcwd()
```

### lambda式
`lambda 引数1, 引数2, ..., 引数n: 実行するステートメント`
```py
>>> func = lambda w, h: w * h
>>> num = func(3, 4)
>>> num
>>> 12
```

### ソート関数を作る
```py
```

### map()
`map(関数, イテラブル)`
```py
def double(x) :
    return x * 2
    
nums = [4, 3, 7, 6, 2, 1]
nums2 = list(map(double, nums))
print(nums2)
```

### イテレーターとは
- イテレーターとは値に含まれている要素を順に１個ずつ取り出せるオブジェクト
- 似ている言葉のイテラブルは要素を順に取り出せるオブジェクトのこと
- イテラブルは取り出された要素の位置を管理しないのに対して、イテレータは要素を１個取り出すごとにどこまで取り出されているかという状態を保持して持っている

### ジェネレーターとは
- イテレーターを作る関数
```py
# ジェネレータ関数
def num_generator():
      n = 0
      while True:
            num = n*n + 2*n + 3 # 数列式
            yield num # ジェネレーターが次に返す値
            n += 1

def do_something(num):
      return (num%2, num%3)

# genジェネレーターを作る
gen = num_generator()
for i in range(1, 10):
      num = next(gen) # ジェネレーターから次の値を取り出す
      result = do_something(num) 
      print(result)
```

```py
# word_quizジェネレーター関数の定義
def word_quiz(word):
      hint = ""
      for letter in word:
            hint += letter # 先に取り出した文字から連結していく
            yield hint

# 出題する
ans = "Python" # 正解
quiz = word_quiz(ans)
while True:
      try:
            hint = next(quiz)
            print(hint)
            word = input("この単語は？：")
            if ans.lower() == word.lower():
                  point = len(ans) - len(hint)
                  print( f"正解です！得点：{point}")
                  break
            else:
                  print("違います。")
      except :
            print("終了です。得点：0")
            break
```

```py
# ジェネレーター式を使う

# oddジェネレーターを作る
# １から５までの奇数を順に返す
odd_gen = (odd for odd in range(1, 6, 2))
```

### ジェネレーターに値を送る
- `yield`を変数に入れ、ジェネレーターオブジェクトにsendメソッドを使って値を送ると変数に値が入る
```py
def testgen():
      n = 0
      while True:
            received = yield n # yieldで返すだけでなく、send()された値を受けてreceivedに代入する
            if received:
                  n = received # send()で受け取った値がreceivedに入っているときに実行する
            else:
                  n = n+1
```

### 初期化メソッド
`def __init__(self, 引数1, 引数2, ...):`

###インスタンス変数を初期化する
`self.変数名 = 初期値`
```py
class Car:
      # 初期化メソッド
      def __init__(self, color="white"):
            self.color = color # 引数で受け取った値を代入
            self.mileage = 0 # 0からスタート
```

### インスタンスを定義する
```py
def メソッド名(self, 引数1, 引数2,...):
      ステートメント
```

### クラスメンバーとインスタンスメンバー
- クラス変数とクラスメソッドは**クラスメンバー**と呼ぶ
- インスタンス変数とインスタンスメソッドは**インスタンスメンバー**と呼ぶ

### クラスメソッドを定義する
```py
@classmethod
def メソッド名(cls, 引数1, 引数2,...):
      ステートメント
```
```py
@classmethod
def countup(cls):
      # クラス変数countを更新
      cls.count += 1
      print(f"出荷台数：{cls.count}")
```
```py
# Carクラス
class Car :
    # クラス変数
    maker = "PEACE"    # 自動車メーカー
    count = 0    # 台数
    
    # クラスメソッド
    @classmethod
    def countup(cls) :
        cls.count += 1
        print(f"出荷台数：{cls.count}")
    
    def __init__(self, color="white"):
      Car.countup() # クラスメソッドcountup()を実行する
      self.mynumber = Car.count # クラス変数を代入
      self.color = color
      self.mileage = 0

    # インスタンスメソッド
    def drive(self, km) :
        self.mileage += km
        msg = f"{km}kmドライブしました。総距離は{self.mileage}kmです。"
        print(msg)
```

### クラスの継承
```py
# datalog.py
from datetime import datetime
class Datalog:
      # 初期化メソッド
      def __init__(self):
            self.loglist = []
      
      # インスタンスメソッド
      def log(self, data):
            # 現在の日時のデータ
            now = datatime.now()
            item = (now, data)
            self.loglist.append(item)

# mydata_test.py
# Datalogクラスが定義してあるモジュールをインポート
from datalog import Datalog
# Datalogを継承したMydataクラス
class Mydata(Datalog):
      def printing(self):
            # スーパークラスのインスタンス変数を取り出す
            for date, data in self.loglist:
                  print(date, data)
```

### スーパークラスの初期化メソッドをオーバーライドしないようにする
```py
# スーパークラス
class Person():
      def __init__(self, name, age):
            self.name = name
            self.age = age

# サブクラス
class Player(Person):
      def __init__(self, name, age, number, position):
            # 第一引数のselfは不要
            super().__init__(name, age)
            self.number = number
            self.position = position
```

### インスタンス変数をprivateにする
- Rubyでいうprivateメソッド。クラス外からアクセスできない
```py
class Person():
      def __init__(self, name):
            # 非公開のインスタンス変数
            self.__name = name
```
- インスタンス変数の値を返すゲッター関数と、値を設定するセッター関数を作ることでクラス外からprivateな変数にアクセスできる

### プロパティを使ってprivateな変数にアクセスする
```py
# ゲッター
@property
def プロパティ(self):
      ステートメント
      return 値　# プロパティの値を返す

# セッター
@プロパティ.setter
def プロパティ(self, value):
      引数valueから設定値を決める
      self.変数 = 値 # プロパティに値を設定する
```
```py
class Goods:
    def __init__(self, name, price):
    # 非公開の__dataインスタンス変数(辞書)
        self.__data = {"name": name, "price": price}

    # nameプロパティ(ゲッター)
    @property
    def name(self):
        return self.__data["name"]

    # nameプロパティ(セッター)
    @name.setter
    def name(self, value):
        self.__data["name"] = value
    
      # priceプロパティ（ゲッター）
    @property
    def price(self):
        price = self.__data["price"]
        # 3桁区切りにして返す
        price_str = f"{price:,}円"
        return price_str
```

### ファイルを開く方法
`open(ファイルのパス, ファイルの処理形式, ファイルの文字コード)`
- r: ファイルの読み込み用に開く
- w: 書き込み用に開く。ファイルが存在する場合は上書きする
- a: 書き込み用に開く。ファイルが存在する場合は追記する
```py
file = "./data/fox.txt"
# ファイルオブジェクトを作る
with open(file) as fileobj:
    # ファイルを読み込む
    text = fileobj.read()
    # 末尾のピリオドを削除しておく
    newtext = text.rstrip(".")
    # スペースで区切ってリストにする
    wordlist = newtext.split(" ")
    print(wordlist)
```

### 折れ線グラフを描く
```py
>>> import matplotlib.pyplot as plt # matplotlibモジュールを読み込む
>>> price = [200, 300, 400, 500, 600] # グラフ化するデータ
>>> count = [31, 29, 25, 28, 26] # グラフ化するデータ
>>> plt.plot(price, count, marker="o") # グラフを描く(x軸price、y軸count、マーカー付き)
>>> plt.title("count-price") # タイトル
>>> plt.xlabel("price") # x軸のラベル
>>> plt.ylabel("count") # y軸のラベル
>>> plt.grid(True) # グリッド
>>> plt.show() # 表示する
```

### sinグラフを描く
```py
import matplotlib.pyplot as plt
import math
>>> X = range(0, 360)
>>> Y = [math.sin(math.radians(d)) for d in X]
>>> plt.plot(X, Y)
>>> plt.show()
```

### 折れ線の種類やマーカを違う種類に設定し、凡例をつける
```py
import matplotlib.pyplot as plt
X = [100, 200, 300, 400, 500,]
Y1 = [40, 65, 80, 100, 90]
Y2 = [34, 56, 75, 91, 79]
Y3 = [25, 47, 68, 76, 73]
plt.plot(X, Y1, marker="o", linestyle = "-", label = "Y1") 
plt.plot(X, Y2, marker="v", linestyle = "--", label = "Y2")
plt.plot(X, Y3, marker="^", linestyle = "-.", label = "Y3") 
plt.legend(loc = "upper left")    # 凡例を作る。凡例の位置をグラフの左上にする
plt.show()       # 表示する
```

### 棒グラフを作成する
```py
import matplotlib.pyplot as plt
labels = ["A", "B", "C", "D", "E", "F", "G", "H", "I", "J"]
x_pos = range(0, 10) # X軸
V = [91, 45, 17, 88, 47, 87, 49, 56, 67, 77] # Y軸
# 縦棒グラフはplt.bar()
plt.bar(x_pos, V, tick_label = labels)    # グラフを描く。tick_labelでX軸に表示するグラフのラベルを指定する
plt.show()    # 表示する

# 横棒グラフはplt.bath()
```

### 積み上げ棒グラフ
```py
import matplotlib.pyplot as plt
labels = ["Green", "Red", "Yellow", "Blue", "Black", "White"]
x_pos = range(0, 6)    # 6本
A = [34, 46, 54, 45, 56, 37]
B = [17, 47, 55, 67, 38, 49]
bar1 = plt.bar(x_pos, A, color = "g")    # グラフAを描く  
bar2 = plt.bar(x_pos, B, color = "c", bottom = A)    # グラフBを描く。
plt.xticks(x_pos, labels, rotation = "vertical")    # X軸ラベル（垂直）
plt.legend((bar1, bar2), ("man", "woman"), loc = "upper right")    # 凡例を作る
plt.show()    # 表示する
```

### 散布図を作成する
```py
import matplotlib.pyplot as plt
import numpy as np
X, Y = np.random.rand(100), np.random.rand(100)    # ランダムな配列を作る
# marker: マーカーの種類
# s: マーカーのサイズ
# color: マーカーの色
# alpha: マーカーの透明度
# linewidths: マーカーの線幅
# edgecolors: マーカーの線色
plt.scatter(X, Y, marker = "o", s = 500, color = "cyan", alpha = 0.5,linewidths = 2, edgecolors = "b")    # グラフを描く
plt.show()    # 表示する
```

### サブプロットに描画する
`add_subplot(行数, 列数, 番号)`
```py
# グラフを左右に並べる

import matplotlib.pyplot as plt
X1, Y1 = range(0, 5), [61, 45, 27, 88, 47]
X2, Y2 = range(0, 5), [17, 39, 46, 40, 27]
labels = ["A", "B", "C", "D", "E"]
fig = plt.figure() # 図を作る
# 1行２列の左
ax1 = fig.add_subplot(1, 2, 1)
ax1.bar(X1, Y1, color="b", tick_label="labels") # グラフの描画
ax1.set_title("dog") # グラフのタイトル
# 1行2列の右
ax2 = fig.add_subplot(1, 2, 2)    # サブプロットを追加する
ax2.bar(X2, Y2, color = "g", tick_label = labels)    # グラフの描画
ax2.set_title("cat")    # グラフのタイトル
plt.show()    # 図を表示する
```
```py
# グラフを上下に分割する

import matplotlib.pyplot as plt
X1, Y1 = range(0, 7), [61, 45, 27, 88, 47, 56, 61]
X2, Y2 = range(0, 7), [17, 39, 46, 40, 27, 35, 41]
labels = ["A", "B", "C", "D", "E", "F", "G"]
fig = plt.figure()    # 図を作る
# 2行1列の上
ax1 = fig.add_subplot(2, 1, 1, facecolor = "cyan")    # サブプロットを追加する
ax1.bar(X1, Y1, color = "b", tick_label = labels)    # グラフの描画
ax1.set_title("snake")    # グラフのタイトル
# 2行1列の下
ax2 = fig.add_subplot(2, 1, 2,  facecolor = "cyan")    # サブプロットを追加する
ax2.bar(X2, Y2, color = "g", tick_label = labels)    # グラフの描画
ax2.set_title("fish")    # グラフのタイトル
plt.tight_layout()    # 下の図のタイトルが重ならないようにする
plt.show()    # 図を表示する
```

### 軸のレンジを調整する
#### 軸の最大値、最小値を指定する
- ax1のグラフを描画した後で`plt.ylim()`を実行してy軸のレンジレンジを取得する。
- 値はタプルの(最小値, 最大値)で帰ってくるので、ymin、ymaxで受ける
```py
import matplotlib.pyplot as plt
X1, Y1 = range(0, 5), [61, 45, 27, 88, 47]
X2, Y2 = range(0, 5), [17, 39, 46, 40, 27]
labels = ["A", "B", "C", "D", "E"]
fig = plt.figure() # 図を作る
# １行２列の左
ax1 = fig.add_subplot(1, 2, 1)
ax1.bar(X1, Y1, color="b", tick_label = labels)
ax1.set_title("dog")
ymin, ymax = plt.ylim() # 現在のY軸のレンジを取得する
ax2 = fig.add_subplot(1, 2, 2)    # サブプロットを追加する
ax2.bar(X2, Y2, color = "g", tick_label = labels)    # グラフの描画
ax2.set_title("cat")    # グラフのタイトル
plt.ylim(ymin, ymax) # Y軸のレンジをax1と合わせる
plt.show()    # 図を表示する
```
#### Y軸を共有する
```py
import matplotlib.pyplot as plt
X1, Y1 = range(0, 5), [61, 45, 27, 88, 47]
X2, Y2 = range(0, 5), [17, 39, 46, 40, 27]
labels = ["A", "B", "C", "D", "E"]
# Y軸を共有する2個のサブプロットを追加する
# nrows: 行数
# ncols: 列数
# sharey: Y軸を共有するサブレイヤを作る
# sharex: X軸を共有するサブレイヤを作る
fig, (ax1, ax2) = plt.subplots(nrows=1, ncols=2, sharey=True)    # 1行2列のサブプロットを追加
ax1.bar(X1, Y1, color = "b", tick_label = labels)    # Y軸を共有したグラフ
ax1.set_title("dog")    # グラフのタイトルを設定
ax2.bar(X2, Y2, color = "g", tick_label = labels)    # Y軸を共有したグラフ
ax2.set_title("cat")    # グラフのタイトルを設定
plt.show()    # 図を表示する
```

### numpyの配列を作る
`array(リスト)`
`array(タプル)`
```py
import numpy as np
>>> a = np.array([1, 2, 3])
>>> a
array([1, 2, 3])

# array()は第二引数でdtype=intのように、型を指定すると、整数値に切り捨てられる
>>> a = np,array([1, 1.5, 2], dtype=int)
>>> a
array([1, 1, 2])
```

### reshape()メソッドを利用して、1次元配列を多次元配列にする
- `reshape(行数, 列数)`と指定して、1次元配列を多次元配列にすることができる
```py
>>> data = [1, 2, 3, 4, 5, 6]
>>> a = np.array(data).reshape(2, 3)
>>> a
array([[1, 2, 3],
      [4, 5, 6]])
```

### ravel()またはflatten()を利用して、多次元配列を1次元配列に戻す
```py
>>>  a = np.array([[0,1], [2,3], [4,5]])
>>> a.ravel()
array([0, 1, 2, 3, 4, 5])
>>> a.flatten()
array([0, 1, 2, 3, 4, 5])
```

### 構造を調べる
```py
# shapeプロパティで何行何列の構造かを調べる
>>> a = np.array([[0,1], [2,3], [4,5]])
>>> a
>>> a.shape
(3, 2)

# ndimプロパティで何次元の配列かを調べる
>>> a.ndim
2
```

### 要素を追加、挿入、削除する
- `append()`,`insert()`, `delete()`を使う
- リストと同名のメソッドだが、リストではリスト自体を直接変更するのに対し、numpyでは新しい配列を作る

`append(配列, 値)`
`append(配列, タプル)`
`append(配列, リスト)`

```py
# 行を追加するときはaxis=0、列を追加するならばaxis=1とする
a = np.array([1, 2, 3, 4, 5, 6]).reshape(2, 3)
b = np.append(a, [[7, 8, 9]], axis = 0)
```
`insert(配列, 位置, 値, axis = None)`
`insert(配列, 位置, リスト, axis = None)`
`insert(配列, 位置, タプル, axis = None)`

### transpose()関数または配列のTプロパティを利用し、転置する
```py
a = np.array([[0,1], [2,3], [4,5]])
np.transpose(a)    # transpose()で転置する
a.T      # Tで転置する
```

### 多次元配列のスライス
- `[行のスライス指定, 列のスライス指定]`
```py
data = [10, 20, 30, 40, 50, 60, 70, 80, 90]
a = np.array(data).reshape(3, 3)
a[:2,]
a[:,1:]
```

### 降順にソート済みの配列を作る
```py
>>> a = np.array([3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5, 8, 9, 7, 9, 3])
>>> a_descend = np.sort(a)[::-1]
>>> a_descend
array([9, 9, 8, 8, 7, 7, 6, 6, 5, 5, 4, 4, 3, 3, 2, 2, 1, 1])
```

### numpy.linalg.norm()を利用して、ベクトルの長さを求める
```py
>>> p0 = np.array((1, 1))
>>> p1 = np.array((6, 4))
>>> A = p1 - p0
>>> a_norm = np.linalg.norm(A)
>>> a_norm
```

### mean()を利用して、平均値を求める
```py
>>> A = np.array([56, 45, 83, 67, 59, 41]).reshape(2, 3)
>>> A.mean() # 全体の平均
>>> A.mean(0) # 各行の平均値
>>> A.mean(1) # 各列の平均値
```

### 標準偏差、偏差値


### dot()を利用して行列の内積を求める
```py
>>> A = np.array([[1, 2],[3, 4]])
>>> B = np.array([[5, 6],[7, 8]])
>>> C = np.dot(A, B)
>>> print(C)
```
### arrange()を利用して、連続番号の配列を作る
`numpy.arrange(start, stop, step)`
```py
>>> import numpy as np
>>> np.arrange(10)
```

### linespace()を利用して、等分割した値の配列を作る
`numpy.linspace(start, stop, 分割数)`
```py
# 0~120を16分割した配列を作る
>>> np.linspace(0, 120, 16)
```

### eye()やidentity()を利用して、単位行列を作る
```py
# ４行４列の単位行列を作る
>>> E = np.identity(4)

# 3行３列の単位行列を作る
>>> E = np.eye(3)

# 整数の単位行列を作りたい場合は、identity()を利用し、第２引数でdtype=intを指定する
>>> E = np.identity(3, dtype=int)
>>> print(E)
```

## [Pythonではじめる機械学習 ―scikit-learnで学ぶ特徴量エンジニアリングと機械学習の基礎](https://www.amazon.co.jp/Python%E3%81%A7%E3%81%AF%E3%81%98%E3%82%81%E3%82%8B%E6%A9%9F%E6%A2%B0%E5%AD%A6%E7%BF%92-%E2%80%95scikit-learn%E3%81%A7%E5%AD%A6%E3%81%B6%E7%89%B9%E5%BE%B4%E9%87%8F%E3%82%A8%E3%83%B3%E3%82%B8%E3%83%8B%E3%82%A2%E3%83%AA%E3%83%B3%E3%82%B0%E3%81%A8%E6%A9%9F%E6%A2%B0%E5%AD%A6%E7%BF%92%E3%81%AE%E5%9F%BA%E7%A4%8E-Andreas-C-Muller/dp/4873117984)まとめ

### sklearnでデータセットを訓練データとテストデータに分割する
- train_test_split関数を使う
- train_test_split関数は分割を行う前にデータセットをシャッフルするので、関数呼び出しのたびに同じ結果が得られるようにrandom_stateパラメータをつける
- 訓練セット75%、テストセット25%の割合で分割する

```python
from sklearn.model_selection import train_test_split
X_train, X_test, y_train, y_test = train_test_split(iris_dataset['data'], iris_dataset['target'], random_state=0)
```

### 教師あり学習は分類と回帰に大別できる
- 分類: 与えられた花の画像からあやめの種類を推測するなど。
- 回帰: 与えられたデータから将来どのようになるかを予測する。

### 汎化とは
- 教師あり学習では訓練データを用いてモデルを構築する。そのモデルが未見のデータに対しても正確に予測できるものならば、訓練セットがテストセットに対して**汎化**できていると言う。

### 過剰適合
- 訓練セットからモデルを作る際は出来るだけ適度に単純化するのが望ましいが、過剰に複雑なモデルを作成してしまうこと。
- 逆に単純化しすぎて訓練セットにもうまく機能しないことを**適合不足**という
