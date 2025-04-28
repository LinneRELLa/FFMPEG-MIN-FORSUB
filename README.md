# FFMPEG-MIN-FORSUB
最小化编译的ffmpeg，仅用于提取封装字幕并为webvtt用于在浏览器或electron应用中正常播放

编译配置
./configure --prefix=/mingw64/custom_ffmpeg_build --disable-everything --enable-ffmpeg --enable-protocol=file --enable-demuxer=mov --enable-demuxer=matroska --enable-demuxer=avi --enable-decoder=subrip --enable-decoder=ass --enable-decoder=mov_text --enable-decoder=dvdsub --enable-encoder=webvtt --enable-muxer=webvtt --enable-small --disable-debug --disable-doc --enable-static --disable-shared --pkg-config-flags=--static --extra-ldflags='-static -static-libgcc -static-libstdc++ -Wl,-Bstatic' --extra-libs='-liconv -lbz2 -lz -lpthread -lm'
