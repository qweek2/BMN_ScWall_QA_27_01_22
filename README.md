# BMN_ScWall_QA_27_01_22
QA for February shifts (2022)

# How to run:

[user@ncx106 BMN]$ root -l -b (don't forget the -b key)  
root [0] .L ScintWall_scan.cpp  
root [1] scan()  

You should set a path to the .root file first  
```
TFile *_file0 = TFile::Open("/path/root_file_name.root");
```

See more advanced comments in the .cpp file  

The *map.pdf* file contains several maps of the ScWall and added automatically to the result.pdf file in the end of the code, if you don't need it just comment the line in the end of the file.
```
gSystem->Exec("pdfunite h1.pdf map.pdf result.pdf");
```
Note that the root map has an inverted X axis unlike the map in *Slide_ScWall.pptx* file, so check the 1st *map.pdf* slide to compare with ScWall histos.
