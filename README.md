# Heart-rate-monitoring
# Abstract
- Heart Rate (HR) is one of the most important Physiological parameter and a vital indicator of people‘s physiological state
- A non-contact based system to measure Heart Rate: real-time application using camera
- Principal: extract heart rate information from facial skin color variation caused by blood circulation 
- Application: monitoring drivers‘ physiological state

# Methods 
- Detect face, align and get ROI using facial landmarks
- Apply band pass filter with fl = 0.8 Hz and fh = 3 Hz, which are 48 and 180 bpm respectively
- Average color value of ROI in each frame is calculate pushed to a data buffer which is 150 in length
- FFT the data buffer. The highest peak is Heart rate
- Amplify color to make the color variation visible 

# Requirements
```
pip install -r requirements.txt
```


# Implementation
```
python GUI.py
```


