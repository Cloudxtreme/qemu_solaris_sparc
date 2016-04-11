# qemu_solaris_sparc
Solaris 8 Sparc Image for qemu-sparc

Example qemu-sparc command:

/usr/local/bin/qemu-system-sparc -monitor telnet:127.0.0.1:3010,server,nowait,ipv4  -nographic -k dk -bios boot_rom/ss20_v2.25_rom -M SS-20 -m 512 -hda sol8sparc10g.disk  -serial telnet:0.0.0.0:3000,server -smp 1,cores=1 -cpu "TI SuperSparc 60" -redir tcp:5023::23 -redir tcp:5021::21 -redir tcp:5020::20

*TIP: 

To create the 7z archive file run the following after downloading: cat xaa xab xac xad xae xaf xag xah xai > sol8sparc.7z

Verify archive:
7z l sol8sparc.7z

Extract archive
7z x sol8sparc.7z
