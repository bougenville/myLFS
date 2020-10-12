# 最小化LFS

## 安装软件

### LFS

### Xorg

### Awesome

### Fonts

Source Cope Pro

noto CJK

powerline

### Emacs

### ibus-libpinyin

### Firefox

### PDF:zathura

### Terminal:elementary terminal /  rxvt-unicode /Tilix

### ZSH

### Exim

### Mutt

### Mine

### TeXLive

## 安装记录

### zsh-5.8

### gcc-9.2.0

### util-macros-1.19.2

### xorgproto-2019.2

### libXau-1.0.9

### libXdmcp-1.1.3

### xcb-proto-1.13

### libxcb-1.13.1

### libpng-1.6.37

### FreeType-2.10.1

### Fontconfig-2.13.1

### Xorg Libraries

### xcb-util-0.4.0

### xcb-util-image-0.4.0

### xcb-util-keysyms-0.4.0

### xcb-util-renderutil-0.3.9

### xcb-util-wm-0.4.1

### xcb-util-cursor-0.1.3

### libxml2-2.9.10

### Wayland-1.18.0

### Wayland-Protocols-1.18

### libuv-1.34.2

### LZO-2.10

### Nettle-3.5.1

### libarchive-3.4.2

### CMake-3.16.4

### MarkupSafe-1.1.1

### Mako-1.1.1

### libdrm-2.4.100

### LLVM-9.0.1

### recommonmark 0.6.0

### Mesa-19.3.4

    meson --prefix=$XORG_PREFIX  -Dbuildtype=release  -Ddri-drivers=auto  -Dgallium-drivers="swrast,svga"  -Dgallium-nine=false -Dglx=dri  -Dosmesa=gallium  -Dvalgrind=false  ..

### xbitmaps-1.1.2

### Xorg Applications

### Xorg Fonts

### XKeyboardConfig-2.29

### Pixman-0.38.4

### libepoxy-1.5.4

### Xorg-Server-1.20.7

### libevdev 1.8.0

### mtdev-1.1.6

### Xorg Evdev Driver-2.10.6

### libinput-1.15.1

### Xorg Libinput Driver-0.29.0

### Xorg Fbdev Driver-0.5.0

### Xorg VMware Driver-13.3.0

### twm-1.0.10

### xterm-353

### xclock-1.0.9

### xinit-1.4.1

### Xorg Legacy

### dbus-1.12.16

### GLib-2.62.4

    meson --prefix=/usr  -Dman=false  -Dselinux=disabled  ..

### gobject-introspection-1.62.0

### ATK-2.34.1

### at-spi2-core-2.34.0

### at-spi2-atk-2.34.1

### FriBidi-1.0.8

### yasm-1.3.0

### libjpeg-turbo-2.0.4

### sgml-common-0.6.3

### UnZip-6.0

### docbook-xml-4.5

### itstool-2.0.6

### shared-mime-info-1.15

### libcroco-0.6.13

### GLU-9.0.1

### Freeglut-3.2.1

### LibTIFF-4.1.0

### gdk-pixbuf-2.40.0

### Graphite2-1.3.13

### ICU-65.1

### Cairo-1.17.2+f93fc72c03e

    /configure --prefix=/usr  --disable-static  --enable-tee --enable-gl --enable-xlib-xcb

### HarfBuzz-2.6.4

### FreeType-2.10.1 pass 2

### Cairo-1.17.2+f93fc72c03e pass 2

### Pango-1.44.7

### sassc-3.6.1

### libxkbcommon-0.10.0

### hicolor-icon-theme-0.17

### libssh2-1.9.0

### Rustc-1.37.0

### Vala-0.48.0

### librsvg-2.46.4

### adwaita-icon-theme-3.36.0

### GTK+-3.24.14

    meson --prefix=/usr  -Dcolord=no  -Dgtk_doc=false  -Dman=false  -Ddemos=false -Dexamples=false -Dtests=false

### DConf-0.34.0 / DConf-Editor-3.34.4

### PyXDG-0.25

### PyCairo-1.19.1

### PyGObject-3.36.0

### ISO Codes-4.4

### ibus-1.5.22

    http://www.unicode.org/Public/emoji/4.0/


    emoji-data.txt
    emoji-sequences.txt
    emoji-test.txt
    emoji-zwj-sequences.txt

    https://github.com/fujiwarat/cldr-emoji-annotation/tree/master/annotations

    安装了zh.xml en.xml

    sed -i 's@/desktop/ibus@/org/freedesktop/ibus@g' \
    data/dconf/org.freedesktop.ibus.gschema.xml

    ./configure --prefix=/usr   --sysconfdir=/etc   --disable-python2 --enable-wayland --enable-vala=yes -with-python=python3

    rm -f tools/main.c

### libpinyin 2.3.0+

    git clone https://github.com/epico/libpinyin.git

    ./configure --prefix=/usr --enable-static=no

### OpenCC 1.05+

    git clone https://github.com/BYVoid/OpenCC.git

    set(BUILD_DOCUMENTATION OFF) at CMakeLists.txt

### SQLite-3.31.1

### ibus-libpinyin 1.11.1

    ./configure --prefix=/usr --enable-static=no --sysconfdir=/etc  --enable-opencc

### luarocks 3.3.1

### lgi 0.9.2-1

### ImageMagick-7.0.9-23

    Delegate library configuration:
    BZLIB             --with-bzlib=yes        yes
    Autotrace         --with-autotrace=no        no
    DJVU              --with-djvu=yes        no
    DPS               --with-dps=yes        no
    FFTW              --with-fftw=yes        no
    FLIF              --with-flif=yes        no
    FlashPIX          --with-fpx=yes        no
    FontConfig        --with-fontconfig=yes    yes
    FreeType          --with-freetype=yes        yes
    Ghostscript lib   --with-gslib=no        no
    Graphviz          --with-gvc=yes        no
    HEIC              --with-heic=yes             no
    JBIG              --with-jbig=yes        no
    JPEG v1           --with-jpeg=yes        yes
    JPEG XL           --with-jxl=yes    no
    LCMS              --with-lcms=yes        no
    LQR               --with-lqr=yes        no
    LTDL              --with-ltdl=yes        yes
    LZMA              --with-lzma=yes        yes
    Magick++          --with-magick-plus-plus=yes    yes
    OpenEXR           --with-openexr=yes        no
    OpenJP2           --with-openjp2=yes        no
    PANGO             --with-pango=yes        yes
    PERL              --with-perl=yes        /usr/bin/perl
    PNG               --with-png=yes        yes
    RAQM              --with-raqm=yes        no
    RAW               --with-raw=yes            no
    RSVG              --with-rsvg=no        no
    TIFF              --with-tiff=yes        yes
    WEBP              --with-webp=yes        no
    WMF               --with-wmf=yes        no
    X11               --with-x=            yes
    XML               --with-xml=yes        yes
    ZLIB              --with-zlib=yes        yes
    ZSTD              --with-zstd=yes        yes

### libxdg-basedir 1.2.0

### libnotify-0.7.9

### startup-notification-0.12

### xcb-util-xrm 1.3

### ldoc-1.4.6-2

### libxcb-errors last

### awesome last

    CMAKE_ARGS="-DCMAKE_INSTALL_PREFIX=/usr -DSYSCONFDIR=/etc" make
    CMAKE_ARGS="-DCMAKE_INSTALL_PREFIX=/usr -DSYSCONFDIR=/etc" make install

    set(GENERATE_MANPAGES OFF)
    set(GENERATE_DOC OFF)

### libconfig last

### compton last

### vbox driver

### noto-fonts

默认配置

    lrwxrwxrwx 1 root root  55  3月 14 06:50 10-hinting-slight.conf -> /usr/share/fontconfig/conf.avail/10-hinting-slight.conf
    lrwxrwxrwx 1 root root  59  3月 14 06:50 10-scale-bitmap-fonts.conf -> /usr/share/fontconfig/conf.avail/10-scale-bitmap-fonts.conf
    lrwxrwxrwx 1 root root  58  3月 14 06:50 20-unhint-small-vera.conf -> /usr/share/fontconfig/conf.avail/20-unhint-small-vera.conf
    lrwxrwxrwx 1 root root  55  3月 14 06:50 30-metric-aliases.conf -> /usr/share/fontconfig/conf.avail/30-metric-aliases.conf
    lrwxrwxrwx 1 root root  49  3月 14 06:50 40-nonlatin.conf -> /usr/share/fontconfig/conf.avail/40-nonlatin.conf
    lrwxrwxrwx 1 root root  31  3月 14 16:30 42-luxi-mono.conf -> ../conf.avail/42-luxi-mono.conf
    lrwxrwxrwx 1 root root  48  3月 14 06:50 45-generic.conf -> /usr/share/fontconfig/conf.avail/45-generic.conf
    lrwxrwxrwx 1 root root  46  3月 14 06:50 45-latin.conf -> /usr/share/fontconfig/conf.avail/45-latin.conf
    lrwxrwxrwx 1 root root  50  3月 14 06:50 49-sansserif.conf -> /usr/share/fontconfig/conf.avail/49-sansserif.conf
    lrwxrwxrwx 1 root root  45  3月 14 06:50 50-user.conf -> /usr/share/fontconfig/conf.avail/50-user.conf
    lrwxrwxrwx 1 root root  46  3月 14 06:50 51-local.conf -> /usr/share/fontconfig/conf.avail/51-local.conf
    lrwxrwxrwx 1 root root  48  3月 14 06:50 60-generic.conf -> /usr/share/fontconfig/conf.avail/60-generic.conf
    lrwxrwxrwx 1 root root  46  3月 14 06:50 60-latin.conf -> /usr/share/fontconfig/conf.avail/60-latin.conf
    lrwxrwxrwx 1 root root  54  3月 14 06:50 65-fonts-persian.conf -> /usr/share/fontconfig/conf.avail/65-fonts-persian.conf
    lrwxrwxrwx 1 root root  49  3月 14 06:50 65-nonlatin.conf -> /usr/share/fontconfig/conf.avail/65-nonlatin.conf
    lrwxrwxrwx 1 root root  48  3月 14 06:50 69-unifont.conf -> /usr/share/fontconfig/conf.avail/69-unifont.conf
    lrwxrwxrwx 1 root root  50  3月 14 06:50 80-delicious.conf -> /usr/share/fontconfig/conf.avail/80-delicious.conf
    lrwxrwxrwx 1 root root  50  3月 14 06:50 90-synthetic.conf -> /usr/share/fontconfig/conf.avail/90-synthetic.conf
    -rw-r--r-- 1 root root 978  3月 14 06:50 README

### strace 5.5

为了解决xterm配置文件的问题

### PCRE2-10.34

### VTE-0.58.3

### ldc last

    安装D语言编译器，先下载预编译程序，然后再编译
    https://github.com/ldc-developers/ldc/releases/download/v1.20.1/ldc2-1.20.1-linux-x86_64.tar.xz
    https://wiki.dlang.org/Building_LDC_from_source
    cmake -G Ninja ../   -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX=/usr -DD_COMPILER=../../ldc2-1.20.1-linux-x86_64/bin/ldmd2

### Module-Build-0.4231

    https://cpan.metacpan.org/authors/id/L/LE/LEONT/Module-Build-0.4231.tar.gz

### libxslt-1.1.34

### po4a last

### GtkD 3.9.0

    make  DCFLAGS='-O -release'  shared-libs shared-gstreamer shared-vte shared-peas
    make prefix=/usr DESTDIR=../gtkd-install  install-shared install-shared-gstreamer install-shared-vte install-shared-peas install-headers install-headers-gstreamer install-headers-vte install-headers-peas

手动安装pkgconfig

    4 -rw-r--r-- 1 root root  127  3月 15 19:31 gstreamerd-3.pc
    4 -rw-r--r-- 1 root root  148  3月 15 19:31 gtkd-3.pc
    4 -rw-r--r-- 1 root root  132  3月 15 19:31 gtkdsv-3.pc
    4 -rw-r--r-- 1 root root  112  3月 15 19:31 peasd-3.pc
    4 -rw-r--r-- 1 root root  109  3月 15 19:31 vted-3.pc

### Links-2.20.2

### xmlto-0.0.28

### xdg-utils-1.1.3

### gsettings-desktop-schemas-3.34.0

解决问题
    Settings schema 'org.gnome.desktop.interface' is not installed

### tilix last

一种方法是用dub安装，网上下载预编译包；另一种方法编译GtkD，然后安装

    ./autogen.sh
    DCFLAGS="-O -inline -release -link-defaultlib-shared" ./configure --prefix=/usr

### ctags 5.8

    http://prdownloads.sourceforge.net/ctags/ctags-5.8.tar.gz

### libgpg-error-1.37

### libgcrypt-1.8.5

### libsecret-0.20.1

    tilix显示没有找到libsecret
    警告依然在，继续安装GnuTLS

### libunistring-0.9.10

### Unbound-1.10.0

    没有启动服务，不太了解此package

### GnuTLS-3.6.12

### VTE-0.58.3 with GnuTLS

解决了 Tilix警告信息

孤立包

    ### libgpg-error-1.37

    ### libgcrypt-1.8.5

    ### libsecret-0.20.1

### LuaFormatter last

VSCode 格式化代码

    https://github.com/Koihik/LuaFormatter

    git clone --recurse-submodules https://github.com/Koihik/LuaFormatter.git
    cd LuaFormatter
    cmake .
    make
    make install

### OpenJPEG-2.3.1

### Poppler-0.86.1

### GLM-0.9.9.7

### GLEW-2.1.0

### slop last

### maim last

### alsa-lib-1.2.2

### alsa-plugins-1.2.2

### alsa-utils-1.2.2

### libogg-1.3.4

### libvorbis-1.3.6

### libsndfile-1.0.28

### Speex-1.2.0

### PulseAudio-13.0

### sound-theme-freedesktop-0.8

打开声音文件失败不知道原因

    paplay /usr/share/sounds/freedesktop/stereo/camera-shutter.oga 
    paplay --list-file-formats

解决了，编译flac，再编译libsndfile-1.0.28就好了

### Libao-1.2.0

    可能是孤立包

### Cbindgen-0.13.1

    for firefox

### vorbis-tools-1.4.0

编译错误，增加了参数
    LIBS="-lm"

### libcanberra-0.30

    孤立包

### dbus-glib-0.110

### GTK+-2.24.32

### Zip-3.0

### Python-2.7.17

### Node.js-12.16.1

    ./configure --prefix=/usr \
    --shared-libuv \
    --shared-openssl \
    --shared-zlib \
    --with-intl=system-icu

### libevent-2.1.11

### NSPR-4.25

### NSS-3.51

### Autoconf2.13

### Firefox-68.6.0

### XML::Simple-2.25

### con-naming-utils-0.8.90

### gnome-icon-theme-3.12.0

### GRUB-2.04

修改configure文件

    DJVU_FONT_SOURCE="/usr/share/fonts/truetype/dejavu"

    ./configure --prefix=/usr \
    --sbindir=/sbin 
    --sysconfdir=/etc \
    --disable-efiemu  \
    --disable-werror \
    --enable-grub-mkfont

    GRUB_GFXMODE=1600x1200
    GRUB_GFXPAYLOAD_LINUX=1600x1200
    GRUB_CMDLINE_LINUX_DEFAULT="vga=0x31F"

### libx86emu

    没用了

### hwinfo last

没用了,已删除

    /usr/bin/inotifywait -mrq --timefmt '%d/%m/%y/%H:%M' --format '%T  %w%f' -e modify,create /usr
    awk '{print $2}' output.txt |uniq -c|awk '{print "rm " $2}'

### libxfce4util-4.14.0

### Xfconf-4.14.1

### libxfce4ui-4.14.1

### URI-1.76

### Exo-0.12.11

### Thunar-1.8.12

### FLAC-1.3.3

libsndfile-1.0.28 必须有flac一起才可以支持oga ogg flac

### id3lib-3.8.3

### libmad-0.15.1b

### cmus last

### JSON-C-0.13.1

### girara last

    meson -Ddocs=disabled --prefix=/usr build

### libseccomp-2.4.3

---for appstream

### glib-networking-2.62.3

### libidn2-2.3.0

### libpsl-0.21.0

### libsoup-2.68.4

### JSON-GLib-1.4.4

### libyaml-0.2.2

### appstream-glib-0.7.17

    meson .. --prefix=/usr -Dbuilder=true -Drpm=false -Dstemmer=false
    没啥用处，找时间删除

### fish-3.1.0

    mkdir build; cd build
    cmake -DCMAKE_INSTALL_PREFIX=/usr -DCMAKE_INSTALL_SYSCONFDIR=/etc ..
    make
    sudo make install

### zathura last

    meson -Ddocs=disabled --prefix=/usr build

### zathura-pdf-poppler last

### Net-tools-CVS_20101030

### bash-completion-2.10

### Boost-1.72.0

    有时间把需要Boost支持的都重新编译一次

### rsync-3.1.3

### libpaper-1.1.24 + nmu5

### Little CMS-2.9

### ghostscript-9.50

Standard Fonts

### Ruby-2.7.0

### libatomic_ops-7.6.10

### GC-8.0.4

### Poppler-0.86.1 with boost

### texlive-2020-source

    rsync -a --delete --exclude=.svn tug.org::tldevsrc/Build/source/ /sources/tmp/tex

    OR

    git clone https://github.com/TeX-Live/texlive-source.git

    export TEXARCH=$(uname -m | sed -e 's/i.86/i386/' -e 's/$/-linux/')
    
    mkdir texlive-build &&
    cd texlive-build

    ../configure                                                    \
        --prefix=/opt/texlive/2020                                  \
        --bindir=/opt/texlive/2020/bin/$TEXARCH                     \
        --datarootdir=/opt/texlive/2020                             \
        --includedir=/opt/texlive/2020/include                      \
        --infodir=/opt/texlive/2020/texmf-dist/doc/info             \
        --libdir=/opt/texlive/2020/lib                              \
        --mandir=/opt/texlive/2020/texmf-dist/doc/man               \
        --disable-native-texlive-build                              \
        --disable-static --enable-shared                            \
        --disable-dvisvgm                                           \
        --with-system-cairo                                         \
        --with-system-fontconfig                                    \
        --with-system-freetype2                                     \
        --with-system-gmp                                           \
        --with-system-graphite2                                     \
        --with-system-harfbuzz                                      \
        --with-system-icu                                           \
        --with-system-libgs                                         \
        --with-system-libpaper                                      \
        --with-system-libpng                                        \
        --with-system-mpfr                                          \
        --with-system-pixman                                        \
        --with-system-zlib                                          \
        --with-system-xpdf                                          \
        --with-system-poppler                                       \
        --with-banner-add=" - BLFS"

../configure                                                    \
        --prefix=/opt/texlive/2020                                  \
        --bindir=/opt/texlive/2020/bin/$TEXARCH                     \
        --datarootdir=/opt/texlive/2020                             \
        --includedir=/opt/texlive/2020/include                      \
        --infodir=/opt/texlive/2020/texmf-dist/doc/info             \
        --libdir=/opt/texlive/2020/lib                              \
        --mandir=/opt/texlive/2020/texmf-dist/doc/man               \
        --disable-native-texlive-build                              \
        --disable-static --enable-shared                            \
        --disable-dvisvgm                                           \
        --with-system-cairo                                         \
        --with-system-fontconfig                                    \
        --with-system-freetype2                                     \
        --with-system-gmp                                           \
        --with-system-graphite2                                     \
        --with-system-harfbuzz                                      \
        --with-system-icu                                           \
        --with-system-libgs                                         \
        --with-system-libpaper                                      \
        --with-system-libpng                                        \
        --with-system-mpfr                                          \
        --with-system-pixman                                        \
        --with-system-zlib                                          \
        --with-system-xpdf                                          \
        --with-system-poppler                                       \
        --with-banner-add=" - BLFS"

    intall-tl

### libksba-1.3.5

### npth-1.6

### libassuan-2.5.3

### GnuPG-2.2.19

### TeXlive 后安装的包

    xpinyin marginnote footmisc titlesec tocvsec2 zhnumber

### Bubblewrap-0.4.0

### Exiv2-0.27.2

### gexiv2-0.12.0

### gnome-autoar-0.2.4

### gnome-desktop-3.34.4

### gstreamer-1.16.2

### gst-plugins-base-1.16.2

### Tracker-2.3.2

### Tracker-miners-2.3.2

### JS-60.8.0

### Polkit-0.116

### polkit-gnome-0.105

### ibgudev-233

### Gvfs-1.42.2

### Evince-3.34.2

    CFLAGS="$CFLAGS -I/opt/texlive/2020/include"      \
    CXXFLAGS="$CXXFLAGS -I/opt/texlive/2020/include"  \
    LDFLAGS="$LDFLAGS -L/opt/texlive/2020/lib"        \
    ./configure --prefix=/usr                         \
                --enable-introspection                \
                --without-gspell                      \
                --disable-static

### tmux 3.1-rc

### Gsl-2.6

### htop-2.2.0

### exim-4.93

    vim Local/Makefile
    AUTH_PLAINTEXT=yes
    AUTH_TLS=yes
    AUTH_CRAM_MD5=yes
    CONFIGURE_FILE=/etc/exim4/exim.conf
    LOG_FILE_PATH=/var/log/exim4/%slog

### GPGME-1.13.1

### Lynx-2.8.9rel.1

### neomutt-20200320

    ./configure --prefix=/usr  --sysconfdir=/etc  --ssl --lua --sqlite  --debug-graphviz --gpgme --autocrypt  --disable-idn --idn2 --zlib --zstd

### Git-2.26.0

### Asciidoc-8.6.9

### Fcron-3.2.1

### msmtp-1.8.7

### Gcr-3.36.0

### gnome-keyring-3.36.0

### t1lib-5.1.2

### libspectre-0.2.8

### Evince-3.36.0

    CFLAGS="$CFLAGS -I/opt/texlive/2020/include"      \
    CXXFLAGS="$CXXFLAGS -I/opt/texlive/2020/include"  \
    LDFLAGS="$LDFLAGS -L/opt/texlive/2020/lib"

### Nautilus-3.36.1.1

### libsigsegv-2.12

### Clisp-2.49

### nginx-1.18.0

    ./configure --prefix=/usr/share/nginx   --sbin-path=/usr/sbin/nginx \
            --modules-path=/usr/lib/nginx/modules   --conf-path=/etc/nginx/nginx.conf        --error-log-path=/var/log/nginx/error.log \
            --http-log-path=/var/log/nginx/access.log    --pid-path=/run/nginx.pid      --lock-path=/var/lock/nginx.lock     --user=nginx     --group=nginx      --build=BLFS             --http-client-body-temp-path=/var/lib/nginx/body             --http-fastcgi-temp-path=/var/lib/nginx/fastcgi             --http-proxy-temp-path=/var/lib/nginx/proxy             --http-scgi-temp-path=/var/lib/nginx/scgi             --http-uwsgi-temp-path=/var/lib/nginx/uwsgi --with-openssl=../openssl-1.1.1g --with-zlib=../zlib-1.2.11 --with-pcre=../pcre-8.44 --with-http_addition_module --with-http_auth_request_module  --with-http_gunzip_module --with-http_dav_module --with-http_gzip_static_module  --with-http_ssl_module  --with-debug

### unrar

### GTK-Doc-1.32
