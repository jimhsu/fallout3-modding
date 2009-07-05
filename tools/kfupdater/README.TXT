                        KfUpdater 2.0
                        =================

    This packages includes an command line application for
      converting custom animation files produced using 
      the Official Civ4 NIF exporter to a version consumable
      by Oblivion or Fallout 3.
    
    
    Usage: 
    
      kfupdater [-opts[modifiers]] <file.kf>
      Convert KF to specified version.

        <Switches>
         -d            Dump Mode      - Output Settings to console
         -s <path>     Settings File  - Initialization settings
         -i <path>     Input File     - Alternate Input File argument
         -v x.x.x.x    Nif Version    - Defaults to input version
         -u x          User Version   - Defaults to input version
         -u2 x         User Version 2 - Defaults to input version
         -p #          Priority       - Default priority for KF Controller upgrades (default: 50)
         -o <path>     Output File    - Defaults to input file with '-out' appended
          
          
    Example:
      
      Converting Oblivion files with default priority of 30:
        kfupdater -p 30 -v 20.0.0.5 -u 11 -u2 11 -i blockidle.kf -o blockidle-out.kf
        
      Converting Fallout 3 files  with default priority of 50:
        kfupdater -p 50 -v 20.2.0.7 -u 11 -u2 34 -i blockidle.kf -o blockidle-out.kf

    Notes:
    
        The -s switch allows for an input file file which defines different priorities based 
           on bone names see the Fallout3_KFSettings.ini for an example.
      
      
      