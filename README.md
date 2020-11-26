1. #### Allow running remotely signed scripts

    ```powershell
    Set-ExecutionPolicy remotesigned -s cu
    ```
    
    Confirm by selecting Yes.


1. #### Install Scoop

    ```powershell
    iex (new-object net.webclient).downloadstring('https://get.scoop.sh')
    ```
    
1. #### Search packages

    ```powershell
    scoop install node
    ```
    
    ```text    
     'main' bucket:
        eventstore (4.1.4) --> includes 'EventStore.ClusterNode.exe'
        node-chakracore (10.13.0)
        nodejs-lts (10.16.3)
        nodejs (12.8.1)
        sliksvn (1.12.0) --> includes 'svn-populate-node-origins-index.exe'   
    ```
    
1. #### Install nodejs-lts

    ```powershell
    scoop install nodejs-lts
    ```
    
    ```text
    Installing '7zip' (19.00) [64bit]
    Downloading https://7-zip.org/a/7z1900-x64.msi (1.7 MB)...
    Checking hash of 7z1900-x64.msi ... ok.
    Extracting 7z1900-x64.msi ... done.
    Linking ~\scoop\apps\7zip\current => ~\scoop\apps\7zip\19.00
    Creating shim for '7z'.
    Creating shortcut for 7-Zip (7zFM.exe)
    '7zip' (19.00) was installed successfully!
    Installing 'nodejs-lts' (10.16.3) [64bit]
    Downloading https://nodejs.org/dist/v10.16.3/node-v10.16.3-win-x64.7z (9.7 MB)...
    Checking hash of node-v10.16.3-win-x64.7z ... ok.
    Extracting node-v10.16.3-win-x64.7z ... done.
    Linking ~\scoop\apps\nodejs-lts\current => ~\scoop\apps\nodejs-lts\10.16.3
    Persisting bin
    Persisting cache
    Running post-install script...
    'nodejs-lts' (10.16.3) was installed successfully!
    ```
    
1. #### Ass extras

    ```powershell
    scoop bucket add extras
    ```
