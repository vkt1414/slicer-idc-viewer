# View IDC data in a locally installed Slicer Instance

## 👷‍♂️🚧 **WARNING**: this repo is in its early development stages. Its functionality may change. Stay tuned for the updates and documentation, and please share your feedback about it by opening issues in this repository🚧

### Steps: 
1. Git clone this repo.
```bash
git clone https://github.com/vkt1414/slicer-idc-viewer.git
```
2. Add the `src` folder as one of the module paths in Slicer settings. Refer to the screenshot below for more information:
   
![Screenshot (17)](https://github.com/vkt1414/slicer-idc-viewer/assets/115020590/48b5a945-3d81-45f8-b7e5-9b1e9f1024e9)

![Screenshot (18)](https://github.com/vkt1414/slicer-idc-viewer/assets/115020590/6136b1de-b117-4b04-b961-57cf14f0a4e9)

![Screenshot (19)](https://github.com/vkt1414/slicer-idc-viewer/assets/115020590/157d50c9-6224-4984-8b94-714a76b86a20)

![Screenshot (20)](https://github.com/vkt1414/slicer-idc-viewer/assets/115020590/666a5513-72c0-43af-80eb-ece9dab0cf76)

3. Restart Slicer
4. Open a URL like `slicer://viewer/?download=$seriesinstanceuid` for example
   ```
   slicer://viewer/?download=1.2.840.113654.2.55.154809705591242159075253605419469935510
   ```
    ### Prerequisties for Ubuntu users: 
    This method requires registering slicer:// as custom web protocol.
    On windows, slicer installation automatically registers custom web protocol for slicer. 
    However, on Ubuntu, edit the `register_slicer_protocol.sh.edit` script to provide the location of the Slicer binary.
    ```
    nano register_slicer_protocol.sh.edit
    ```
    save it as register_slicer_protocol.sh
    
    
    Make this file an executable
    ```
    chmod +x register_slicer_protocol.sh
    ```
    Run the script
    ```
    ./register_slicer_protocol.sh
    ```

