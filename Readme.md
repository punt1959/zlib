# zlib-1.2.11 
This has been modified to make static libraries only from the needed files of the official [zlib]( https://github.com/madler/zlib) project.  
## To build:  
### Visual Studio 2022  
Traverse to .\ide\vs2022\zlib folder, and open zlib.sln.  
Select either Release/Debug in Visual Studio, and Build it.  
### CMake  
1. Create a build location  
   - Enter:  `mkdir build`  
2. Move to that locations  
   - Enter:  `cd build`  
3. Create the make files   
   - **Windows**  (from a Developers command prompt)  
      - Enter:  `cmake .. -DCMAKE_BUILD_TYPE=Release -G"NMake Makefiles"`  
    - **macOS**  
      - Enter:  `cmake .. -DCMAKE_BUILD_TYPE=Release -G"Unix Makefiles"`  
    - **All Other Operation Systems**  
      - Enter:  `cmake .. -DCMAKE_BUILD_TYPE=Release`  
4. Build the system entering:  `cmake --build . --config Release`  
5. The resulting product will be in the current (build) directory    
