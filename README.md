# vmware-fusion-bootcamp

Sometimes VMWare Fusion says it cannot find your Boot Camp partition, even though the partition does exist and you can boot into it when starting your Mac.

Using this script should let you create a Boot Camp VM.

## Requirements

- VMWare Fusion
- An existing Boot Camp install

## Instructions

1. [Download this repository](https://github.com/mikew/vmware-fusion-bootcamp/archive/master.zip)
2. Extract `vmware-fusion-bootcamp-master.zip`
3. Run `fusion-make-bootcamp` in a terminal

    > Note if your Boot Camp partition is not on your internal drive you can pass the disk as the first argument to this script:

    ```bash
    fusion-make-bootcamp /dev/disk1
    ```

4. There should now be a Boot Camp VM on your desktop

## BitLocker

If you enable BitLocker after creating the VM, Fusion might say it can't find it anymore. 
Just run the script again.