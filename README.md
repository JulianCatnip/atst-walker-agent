# AT-ST Walker Project Guide
## Unity Version
Please use following Unity-Version:
| Version |
| ------ |
| 2020.3.7f1 |
## ML-Agents Set-up
### Compatible Versions

| Version | Python Package | Unity Package |
| ------ | ------ | ------ |
| Release 17 | 0.26.0 | 2.0.0 |

Source-Files: [https://github.com/Unity-Technologies/ml-agents/tree/release_17](https://github.com/Unity-Technologies/ml-agents/tree/release_17)

### Installing ML-Agents dependencies in Unity

- If you open this project in Unity, this error might occur:

![Unity Error](/img/unity-error.png)

- To solve it, download the Source-Files of [ML-Agents Release 17](https://github.com/Unity-Technologies/ml-agents/tree/release_17) mentioned before.
- In Unity: 
    - Click "Continue" (Error window) and import missing packages manually over **Window > Package Manager**.
    
    ![Package Manager 1](/img/unity-package-manager-1.png)

    - Click the plus and choose **Add package from disk...**

    ![Package Manager 2](/img/unity-package-manager-2.png)

    - Find and open the **package.json** in the previously downloaded and unzipped package at **ml-agents > com.unity.ml-agents.extensions**.

    ![Package Manager 3](/img/unity-package-manager-3.png)

### Installing ML-Agents dependencies for Python

- In your Python env use 
    - `python -m pip install mlagents==0.26.0` to install the correct ML-Agents version, and 
    - `pip3 install torch -f https://download.pytorch.org/whl/torch_stable.html` to download PyTorch.
