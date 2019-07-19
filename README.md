# Lisp(S-expression) with output and inout mark
有输出标记和输入输出半双工标记的 Lisp (S-expression)

## Description in English

```
(RDS_0 ↑DS_3 ↕DS_2 DS_1)
;; Or
(RDS_0 ^DS_3 *DS_2 DS_1)
;; Distinguish output and inout from parameters when being called
```

DS_1 stands for input, with no special mark

DS_2 stands for inout, with ↕ or * mark

DS_3 stands for output，with ↑ or ^ mark

The reason of this design comes from [lisp 的设计失误之二: 输入输出明确性](https://zhuanlan.zhihu.com/p/52993771)

## 中文描述

```
(RDS_0 ↑DS_3 ↕DS_2 DS_1)
;; 或者
(RDS_0 ^DS_3 *DS_2 DS_1)
;; 调用时，从参数中，区分输出以及输入输出半双工`
```

DS_1 是输入项，不需要特别标识

DS_2 是输入输出半双工项，需要 ↕ 或者 * 标识

DS_3 是输出项，需要 ↑ 或者 ^ 标识

设计理由来自文章 [lisp 的设计失误之二: 输入输出明确性](https://zhuanlan.zhihu.com/p/52993771)
