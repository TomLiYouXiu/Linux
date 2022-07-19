# 新建，保存和退出

~~~shell
i 	#进入编辑模式
esc #正常退出
: 	#命令行退出
:q 	#仅退出
:q!	#不保存退出
:wq #保存推出
~~~

# 导航与编辑

~~~shell
#正常模式下移动
i	#插前
I	#在最前插入
a	#附后
A	#在最后插入
hjkl#左下上右
o	#新增下一行
O	#新增上一行
G	#到最后一行
gg 	#到第一行
----------------
#没有设置绝对行数下
*j	#向下移动几行
----------------
#设置绝对行数
#set relativenumber
*j	#下几行
*k	#上几行
----------------
yy	#复制当前的一行，在输入p显示复制的内容
dd	#删除当前的一行
.	#重复当前的操作
u	#撤销当前的操作
ctrl+r#恢复当前的操作
dw	#删除单词
cw	#改变字符
w	#下个单词的首部
e	#下个单词的尾部
b	#上个单词的首部
/	#搜索
:%s/旧字符/新字符/g#替换字符
yw	#复制单词
p	#粘贴
*p	#粘贴几次
ci{	#删除{}里的内容，也可以[],()
ctrl+v#视觉模式，可视块
shift+v#可视化行
~~~

~~~shell
查看版本
[root@iZfdjfsqewlu0jZ home]# vim --version
VIM - Vi IMproved 8.0 (2016 Sep 12, compiled Sep 22 2021 11:10:49)
包含补丁: 1-1763
修改者 <bugzilla@redhat.com>
编译者 <bugzilla@redhat.com>
巨型版本 无图形界面。  可使用(+)与不可使用(-)的功能:
+acl               +farsi             +mouse_sgr         -tag_any_white
+arabic            +file_in_path      -mouse_sysmouse    -tcl
+autocmd           +find_in_path      +mouse_urxvt       +termguicolors
-autoservername    +float             +mouse_xterm       +terminal
-balloon_eval      +folding           +multi_byte        +terminfo
+balloon_eval_term -footer            +multi_lang        +termresponse
-browse            +fork()            -mzscheme          +textobjects
++builtin_terms    +gettext           +netbeans_intg     +timers
+byte_offset       -hangul_input      +num64             +title
+channel           +iconv             +packages          -toolbar
+cindent           +insert_expand     +path_extra        +user_commands
-clientserver      +job               +perl/dyn          +vertsplit
-clipboard         +jumplist          +persistent_undo   +virtualedit
+cmdline_compl     +keymap            +postscript        +visual
+cmdline_hist      +lambda            +printer           +visualextra
+cmdline_info      +langmap           +profile           +viminfo
+comments          +libcall           +python/dyn        +vreplace
+conceal           +linebreak         +python3/dyn       +wildignore
+cryptv            +lispindent        +quickfix          +wildmenu
+cscope            +listcmds          +reltime           +windows
+cursorbind        +localmap          +rightleft         +writebackup
+cursorshape       +lua/dyn           +ruby/dyn          -X11
+dialog_con        +menu              +scrollbind        -xfontset
+diff              +mksession         +signs             -xim
+digraphs          +modify_fname      +smartindent       -xpm
-dnd               +mouse             +startuptime       -xsmp
-ebcdic            -mouseshape        +statusline        -xterm_clipboard
+emacs_tags        +mouse_dec         -sun_workshop      -xterm_save
+eval              +mouse_gpm         +syntax            
+ex_extra          -mouse_jsbterm     +tag_binary        
+extra_search      +mouse_netterm     +tag_old_static    
     系统 vimrc 文件: "/etc/vimrc"
     用户 vimrc 文件: "$HOME/.vimrc"
 第二用户 vimrc 文件: "~/.vim/vimrc"
      用户 exrc 文件: "$HOME/.exrc"
       defaults file: "$VIMRUNTIME/defaults.vim"
         $VIM 预设值: "/etc"
  $VIMRUNTIME 预设值: "/usr/share/vim/vim80"
编译方式: gcc -c -I. -Iproto -DHAVE_CONFIG_H     -O2 -g -pipe -Wall -Werror=format-security -Wp,-D_GLIBCXX_ASSERTIONS -fexceptions -fstack-protector-strong -grecord-gcc-switches -specs=/usr/lib/rpm/redhat/redhat-hardened-cc1 -specs=/usr/lib/rpm/redhat/redhat-annobin-cc1 -m64 -mtune=generic -fasynchronous-unwind-tables -fstack-clash-protection -fcf-protection -D_GNU_SOURCE -D_FILE_OFFSET_BITS=64 -I/usr/include/python3.6m -U_FORTIFY_SOURCE -D_FORTIFY_SOURCE=1       
链接方式: gcc   -L. -Wl,-z,relro  -Wl,-z,now -specs=/usr/lib/rpm/redhat/redhat-hardened-ld -fstack-protector-strong -rdynamic -Wl,-export-dynamic -Wl,--enable-new-dtags -Wl,-z,relro -Wl,-z,now -specs=/usr/lib/rpm/redhat/redhat-hardened-ld  -Wl,-z,relro  -Wl,-z,now -specs=/usr/lib/rpm/redhat/redhat-hardened-ld -L/usr/local/lib -Wl,--as-needed -o vim        -lm  -lselinux   -lncurses -lacl -lattr -lgpm -ldl   -Wl,--enable-new-dtags -Wl,-z,relro -Wl,-z,now -specs=/usr/lib/rpm/redhat/redhat-hardened-ld -Wl,-z,relro -Wl,-z,now -specs=/usr/lib/rpm/redhat/redhat-hardened-ld -fstack-protector-strong -L/usr/local/lib  -L/usr/lib64/perl5/CORE -lperl -lpthread -lresolv -ldl -lm -lcrypt -lutil -lc

#配置行号显示
在配置文件中 "/etc/vimrc" 输入set number 
绝对行数 set relativenumber
~~~

