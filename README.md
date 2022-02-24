# AT-ST Walker Machine Learning Agent using Unity ML-Agents
## About the project
- Find the **full agent concept**
  - in German (original): <a target="_blank" href="https://www.juliancatnip.de/documents/at-st_walker/ATST-Walker_Konzept.pdf" title="ML Agent Concept in German">ATST-Walker_Konzept.pdf</a>
  - in English (DeepL translated): <a target="_blank" href="https://www.juliancatnip.de/documents/at-st_walker/ATST-Walker_Concept_EN.pdf" title="ML Agent Concept in English">ATST-Walker_Concept_EN.pdf</a>
## Technical details
- Unity Version
  - 2020.3.7f1

- Required packages
  - ML Agents (2.0.0-exp.1)
  - ML Agents Extensions (0.4.0-preview)

- Project repository
  - Assets/
    - **AT-ST_Walker/**
    - ML-Agents/

## ML-Agents Set-up
### Compatible Versions

| Version | Python Package | Unity Package |
| ------ | ------ | ------ |
| Release 17 | 0.26.0 | 2.0.0 |

Source-Files: [https://github.com/Unity-Technologies/ml-agents/tree/release_17](https://github.com/Unity-Technologies/ml-agents/tree/release_17)

### Installing ML-Agents dependencies in Unity

- If you open this project in Unity, this error might occur:

![Unity Error](/readme_src/unity-error.png)

- To solve it, download the Source-Files of [ML-Agents Release 17](https://github.com/Unity-Technologies/ml-agents/tree/release_17) mentioned before.
- In Unity: 
    - Click "Continue" (Error window) and import missing packages manually over **Window > Package Manager**.
    
    ![Package Manager 1](/readme_src/unity-package-manager-1.png)

    - Click the plus and choose **Add package from disk...**

    ![Package Manager 2](/readme_src/unity-package-manager-2.png)

    - Find and open the **package.json** in the previously downloaded and unzipped package at **ml-agents > com.unity.ml-agents.extensions**.

    ![Package Manager 3](/readme_src/unity-package-manager-3.png)

### Installing ML-Agents dependencies for Python

- In your Python env use 
    - `python -m pip install mlagents==0.26.0` to install the correct ML-Agents version, and 
    - `pip3 install torch -f https://download.pytorch.org/whl/torch_stable.html` to download PyTorch.

## Results
![AT-ST Walker agent](https://www.juliancatnip.de/images/at-st_walker/04.gif)
*This is not the final result, just the output after the first incorrect test run and I love it*
[![Youtube Video of the walking AT-ST Walker Agent](https://img.youtube.com/vi/JQzt69A6v3s/0.jpg)](https://www.youtube.com/watch?v=JQzt69A6v3s)
