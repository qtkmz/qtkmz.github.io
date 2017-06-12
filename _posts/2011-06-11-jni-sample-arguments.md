---
layout: post
title:  "メソッドの引数に変数を渡す - JNI サンプル"
date:   2011-06-11 00:52:28 +0900
categories: java c jni
---
Java のクラスメソッドに、変数を渡すサンプルを書いてみた。
int, String, String[] の 3 つ。

基本的には、Java に渡すために変数を変換してあげるくらいで、それ程手間ではないかな。動くからって今のコードが正しいと言えないものなので、いくつか確認は必要かな。

あと、エラー処理が足りない。

## int の場合
http://qtakamitsu-snippet.googlecode.com/svn/trunk/lang/c/jni/args_int/

## String の場合
http://qtakamitsu-snippet.googlecode.com/svn/trunk/lang/c/jni/args_string/

## String[] の場合
http://qtakamitsu-snippet.googlecode.com/svn/trunk/lang/c/jni/args_string_array/
