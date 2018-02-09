安装
npm install stylus -g

将.styl文件导出.css:
stylus -w style.styl -o style.css

――――――――――――――――――
生成CSS
命令行中
建立一个stylusExample/，再在里面建立 src 目录专门存放 stylus 文件，在里面建立 example.styl 文件。然后在 stylusExample 目录下面执行下面命令

$ stylus --compress src/

输出compiled src/example.css ，这个时候表示你生成成功了，带上--compress参数表示你生成压缩的CSS文件。

$ stylus --css css/example.css css/out.styl CSS转换成styl 
$ stylus help box-shadow CSS属性的帮助 
$ stylus --css test.css 输出基本名一致的.styl文件
――――――――――――――――――――――
$ stylus -h

  Usage: stylus [options] [command] [< in [> out]]
                [file|dir ...]

  Commands:

    help [<type>:]<prop> Opens help info at MDN for <prop> in
                         your default browser. Optionally
                         searches other resources of <type>:
                         safari opera w3c ms caniuse quirksmode

  Options:

    -i, --interactive       Start interactive REPL
    -u, --use <path>        Utilize the Stylus plugin at <path>
    -U, --inline            Utilize image inlining via data URI support
    -w, --watch             Watch file(s) for changes and re-compile
    -o, --out <dir>         Output to <dir> when passing files
    -C, --css <src> [dest]  Convert CSS input to Stylus
    -I, --include <path>    Add <path> to lookup paths
    -c, --compress          Compress CSS output
    -d, --compare           Display input along with output
    -f, --firebug           Emits debug infos in the generated CSS that
                            can be used by the FireStylus Firebug plugin
    -l, --line-numbers      Emits comments in the generated CSS
                            indicating the corresponding Stylus line
    -m, --sourcemap         Generates a sourcemap in sourcemaps v3 format
    --sourcemap-inline      Inlines sourcemap with full source text in base64 fo                                                                                                                                                                                               rmat
    --sourcemap-root <url>  "sourceRoot" property of the generated sourcemap
    --sourcemap-base <path> Base <path> from which sourcemap and all sources are                                                                                                                                                                                                relative
    -P, --prefix [prefix]   prefix all css classes
    -p, --print             Print out the compiled CSS
    --import <file>         Import stylus <file>
    --include-css           Include regular CSS on @import
    -D, --deps              Display dependencies of the compiled file
    --disable-cache         Disable caching
    --hoist-atrules         Move @import and @charset to the top
    -r, --resolve-url       Resolve relative urls inside imports
    --resolve-url-nocheck   Like --resolve-url but without file existence check
    -V, --version           Display the version of Stylus
    -h, --help              Display help information


