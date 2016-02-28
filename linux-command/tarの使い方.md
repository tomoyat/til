# 引数の意味っぽいの

```sh
# manから抜粋
SYNOPSIS
     tar [bundled-flags <args>] [<file> | <pattern> ...]
     tar {-c} [options] [files | directories]
     tar {-r | -u} -f archive-file [options] [files | directories]
     tar {-t | -x} [options] [patterns]
```

`tar -c`とかでやる方法もあるっぽい

* `-c`: 新しいアーカイブを作る
* `-x`: アーカイブを展開する
* `-f file`: 固める先のfile名 or 展開するfile名
* `-z`: 結果をgzipする
* `-v`: 処理してるfileを表示する

# フォルダをtar.gzにする

```
tar -c -z -f dist.tar.gz source
```

# tar.gzから戻す

```
tar -x -f source.tar.gz
```
