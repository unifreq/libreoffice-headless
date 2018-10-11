# libreoffice-headless
base on opensuse
set timezone to Asia/Shanghai
add busybox
add oracle jre8
add libreoffice 6.04
delete some unused files and directories
total size is 7xxMB

usage example:
1. convert to pdf file use shell command

run -it  -v /usr/share/fonts:/usr/share/fonts -v /usr/local/share/fonts:/usr/local/share/fonts -v /tmp:/tmp unifreq/libreoffice-headless --invisible --headless --convert-to pdf /tmp/demo.doc --outdir /tmp

2. run libreoffice-headless daemon

run -d -v /usr/share/fonts:/usr/share/fonts -v /usr/local/share/fonts:/usr/local/share/fonts -v /tmp:/tmp unifreq/libreoffice-headless --
