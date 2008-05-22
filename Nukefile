(task "clobber" => "clean" is
	(SH "rm nug.m")
	(SH "rm nug"))


(task "install" => "default" is
	(SH "sudo rm -f /usr/local/bin/nug")
	(SH "sudo ditto nug /usr/local/bin/nug"))

(task "default" is
	(SH "nubake nug.nu -s")
	(SH "gcc nug.m -o nug -framework Cocoa -framework Nu"))

(task "doc" is (SH "nudoc"))
