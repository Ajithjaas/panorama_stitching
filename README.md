# Phase 1 - Traditional Method
## Steps in Traditional Method:
    - Corner Detection
    - Adaptive Non-Maximal Suppression (ANMS)
    - Feature Descriptor
    - Feature Matching
    - RANSAC for Outlier Rejection
    - Blending Images

Navigate the below folder:
```json
cd ../Phase1/Code/
```
Run the follwing code:
```json
python Wrapper.py
```

# Phase 2 - Deep Learning Approach
## Instructions to run the code
Please make sure you are in the same directory as the code files in order to execute them in the command prompt. If not, use cd/../loc to navigate to the location of the Python files.

Navigate the below folder:
```json
cd ../Phase2/Code/
```
## Creating the data
### The following command must be entered into the command prompt to create Training data:
```json
python Wrapper.py --NumFeatures 64 --Data Train
```
### The following command must be entered into the command prompt to create Testing Data:
```json
python Wrapper.py --NumFeatures 64 --Data Test
```
### The following command must be entered into the command prompt to run training:
```json
python Train.py --NumFeatures 64 --ModelType Sup
```
Based on the Model to run, the --ModelType can either Sup for supervised network and Unsup for Unsupervised Network.
In case you need more information regarding the parse arguments for a particular file, you can run the following code:
```json
python Train.py -h
```
### The following command must be entered into the command prompt to run testing:
```json
 python Test.py --NumFeatures 64
 ```
