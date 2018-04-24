# DvrConf.txt
================================
	DVR Config TXT [Ver 0.01]
================================
[MODEL]:0x8044
[BOARD]:0x0
[LOCAL]:0x0
[RESOL]:0x4
[MAC]:00:16:6C:F1:8F:06
================================

# sysconf - bootloader
DVR ip adress : 192.168.75.194
server ip adress : 192.168.75.99
gateway ip adress : 192.168.75.1
eth0 mac : 00:09:18:4C:88:4F
video out : 0x04
NTSC/PAL : NTSC
host name : Entry_detroit
Board ID : 0x8061
Locale : 0x0002

mac 주소는 6바이트(48비트), 8비트x6개


-------------------------------------------------------------------------------

# protocol buffers


## installation 
https://github.com/google/protobuf/blob/master/src/README.md


## Textual representation
> Textual representation of a protocol buffer.
> This is *not* the binary format used on the wire.

<pre><code>
person {
  name: "John Doe"
  email: "jdoe@example.com"
}
</code></pre>




## Compiling dependent packages of protocol buffers 

<pre><code>
dm8:~/update_dvr_conf/pb_test$ pkg-config --cflags protobuf
-pthread -I/usr/local/include
dm8:~/update_dvr_conf/pb_test$ pkg-config --libs protobuf
-L/usr/local/lib -lprotobuf -pthread -lpthread
dm8:~/update_dvr_conf/pb_test$ pkg-config --cflags protobuf
-pthread -I/usr/local/include
dm8:~/update_dvr_conf/pb_test$ pkg-config --cflags --libs protobuf
-pthread -I/usr/local/include -L/usr/local/lib -lprotobuf -pthread -lpthread
</code></pre>
