<!--
>=============================================================================
>     FileName: mark.md
>         Desc: 
>       Author: Lolly
>        Email: cclolly@gmail.com
>     HomePage: 
>      Version: 0.0.1
>   LastChange: 2014-02-18 12:03:14
>      History:
>=============================================================================
-->

Mark Talk
=========
> 代码备注的符号表示法  
> 注释以及代码都是以 PHP 为例

## Version ##
0.01

## Function ##
> Function comments

### Table ###
| Mark        | Info           | Info (中文)    | Demo                                          |
|-------------|----------------|----------------|-----------------------------------------------|
|             | general        | 常规           | // comments...                                |
| =>          | return         | 返回信息       | // =>                                         |
| ->          | output         | 直接输出       | // -> (string)$string                         |
| ~>          | run            | 运行           | // ~> $function                               |
| (type)      | type           | 类型           | // => (string/array/int/boole/float/...)      |
| $w          | variable name  | 变量名称       | // => (string)$error                          |

### Demo ###
```php
function return($obj) // => (string)$string
{
  // ...
  return $string;
}
```
```php
function output($obj) // -> (string)$string
{
  // ...
  echo $string;
}
```
```php
function run($obj) // ~> $demo
{
  // ...
  $demo();
}
```

## Code ##
> Code comments

### Table ###
| Mark        | Info           | Info (中文)    | Demo (中文)                                   |
|-------------|----------------|----------------|-----------------------------------------------|
|             | general        | 常规描述       | // 代码的说明                                 |
| #\*         | important      | 关键代码       | // #\* 需反复确认，异常将导致系统崩溃         |
| #!          | error          | 错误           | // #! 严重错误，先注释掉                      |
| #?          | interrogatory  | 疑惑           | // #? 这个部分不太理解，理由...               |
| #~          | temp           | 需要被修改     | // #~ 临时功能，需补充 XX 在这里，以完善      |
| #&          | planned        | 计划功能       | // #& 计划在这里加入权限验证                  |
| #$          | unstable       | 未充分测试     | // #$ 还没测试在 XX 情况下的表现              |
| #^          | bottleneck     | 性能瓶颈       | // #^ 这里有性能问题，需要优化                |
| #%          | rework         | 重构           | // #% 这个需要用 XX 重构                      |
| # w +       | function begin | 特别功能块开始 | // # Lolly +                                  |
| # w -       | function end   | 特别功能块结束 | // # Lolly -                                  |
| ::          | author         | 备注人         | // #~ 权限表待补充::Lolly                     |
| @           | time           | 备注时间       | // #$ 未测试::Lolly@20140123                  |
| ^           | local          | 备注地点       | // #% 明天重构::Lolly^home@20140123           |
| #\[w\]\(u\) | link           | 链接           | // #\[参考地址\]\(http://www.alloyteams.com\) |

