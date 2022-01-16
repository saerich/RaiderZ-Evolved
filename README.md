# RaiderZ Evolved Project

### Requirements:
- If you would like to open the not upgraded projects: Visual Studio 2008 with SP1 Update (https://stackoverflow.com/questions/17108102/download-and-install-visual-studio-2008)
- Visual Studio 2019 v16.10.1 (https://visualstudio.microsoft.com/downloads/)
  - With the following workloads selected:
  - Desktop development with C++
  - .NET desktop development
  - Game development with C++
- DirectX 9 SDK (https://www.microsoft.com/en-gb/download/details.aspx?id=6812)
- Microsoft SQL Server 2019 (https://www.microsoft.com/en-us/sql-server/sql-server-downloads)
- Git (https://git-scm.com/)

### Cloning:
1. Using git (either in visual studio, command line, git tortoise, or something else).
3. Clone the RaiderZ-Evolved repository: ```git clone https://github.com/saerich/RaiderZ-Evolved.git``` to a suitable folder.
4. Make sure all modules are on the master branch.

### Building Game Client:
1. Open the ```source/Game``` folder.
2. Open the ```Game.sln``` file.
3. Select the ```Release_publish``` configuration or ```Debug``` configuration for debugging.
4. Go to Build > Build Solution.

### Debugging the Game Client:
1. Right click the ```GameApp``` project and click ```Set as Startup Project```
2. Right click ```GameApp``` project and click ```Properties```
3. Make sure the configuration is set to Debug.
4. Under ```Configuration Properties``` select ```Debugging```
5. Make sure that the command path is leading to the client .exe file.
6. Make sure the working directory is leading to the client folder.
7. Set command arguments to ```launch test2 127.0.0.1``` where ```test2``` is the name of the account you're logging into.

### Building the Server:
1. The server source code can be found in ```source/Server```
2. You are required to build ```AppServer```, ```GameServer```, ```LoginServer```, and ```MasterServer```
3. Open ```source/Server/AppServer/AppServer.sln``` and build using either ```Release_publish``` or ```Debug```
4. Open ```source/Server/GameServer/GameServer.sln``` and build using either ```Release_publish``` or ```Debug```
5. Open ```source/Server/LoginServer/LoginServer.sln``` and build using either ```Release_publish``` or ```Debug```
6. Open ```source/Server/MasterServer/MasterServer.sln``` and build using either ```Release_publish``` or ```Debug```

Note: All testing was performed with ```_Console``` project. The ```_App``` project may or may not work.