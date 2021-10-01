---
marp: true
---

<!-- class: invert -->

# Enhance assistance for reversing Go 
## @hijiki51

![bg right w:200](images/gopher.png)

---

# Background

- Go製のマルウェアが増えてきている

- 独自のランタイムを持つため、解析が正常に行われない

--- 
# TODO: image

---

# Background

- [felberj/gotools](https://github.com/felberj/gotools)

- GhidraでのGoバイナリの解析をサポートしてくれる
    - 関数名の復元
    - 一部型の復元
    - 返り値の復元
---

# Background
## Go1.16
- pclntabの構造の変更
    - 関数アドレス、関数名等の情報を持つ
- 関数名の復元ができなくなる

---

# Background
## Go 1.17
- 関数呼び出し規約の変更
    - 引数/返り値をレジスタで扱うように
- 返り値の復元ができなくなる
