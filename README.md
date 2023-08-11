# efibootmgr cheat sheet

 - List:
   - `efibootmgr`
 - List verbose:
   - `efibootmgr -v`
   - `efibootmgr --verbose`
 - Create:
   - `efibootmgr -c -d /dev/sda1 -l '\EFI\OC\OpenCore.efi' -L 'OpenCore'`
   - `efibootmgr --create --disk /dev/sda1 --loader '\EFI\OC\OpenCore.efi' --label 'OpenCore'`
 - Delete:
    - `efibootmgr -b 6 -B`
    - `efibootmgr -b 0006 -B`
    - `efibootmgr --bootnum 0006 --delete-bootnum`
