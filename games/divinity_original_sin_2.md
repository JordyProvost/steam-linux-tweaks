Game does not start, or start and crash immediately.

Install winetricks under root :

```apt install winetricks```

Execute this with normal user :

```cd ~/.steam/steam/steamapps/common/"Divinity Original Sin 2"/ && mv ./bin ./bin.bak && ln -s DefEd/bin bin && mv ./Data ./Data.bak && ln -s DefEd/Data Data && cd bin && mv ./SupportTool.exe ./SupportTool.bak && ln -s EoCApp.exe SupportTool.exe && WINEPREFIX=~/.steam/steam/steamapps/compatdata/435150/pfx/ winetricks xact```

Tested with GE-proton7-41 (installed with ProtonUp-Qt)
