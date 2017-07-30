# The ThinkPHP5 Image Package

[![Build Status](https://img.shields.io/travis/top-think/think-image.svg)](https://travis-ci.org/top-think/think-image)
[![Coverage Status](https://img.shields.io/codecov/c/github/top-think/think-image.svg)](https://codecov.io/github/top-think/think-image)
[![Downloads](https://img.shields.io/github/downloads/top-think/think-image/total.svg)](https://github.com/top-think/think-image/releases)
[![Releases](https://img.shields.io/github/release/top-think/think-image.svg)](https://github.com/top-think/think-image/releases/latest)
[![Releases Downloads](https://img.shields.io/github/downloads/top-think/think-image/latest/total.svg)](https://github.com/top-think/think-image/releases/latest)
[![Packagist Status](https://img.shields.io/packagist/v/top-think/think-image.svg)](https://packagist.org/packages/topthink/think-image)
[![Packagist Downloads](https://img.shields.io/packagist/dt/top-think/think-image.svg)](https://packagist.org/packages/topthink/think-image)

## 特别说明

修改至topthink/think-image 扩展
将发生错误时抛出异常，改为返回错误信息，然后调用时根据错误信息进行下一步处理，以免造成页面显示异常错误无法正常访问！！！
 
## 安装

> composer require topthink/think-image

## 使用

~~~
$image = \think\Image::open('./image.jpg');
或者
$image = \think\Image::open(request()->file('image'));


$image->crop(...)
    ->thumb(...)
    ->water(...)
    ->text(....)
    ->save(..);

~~~