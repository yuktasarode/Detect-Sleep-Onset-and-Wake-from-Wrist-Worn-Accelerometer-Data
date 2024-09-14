# Detect-Sleep-Onset-and-Wake-from-Wrist-Worn-Accelerometer-Data

Wrist-worn accelerometers are capable of detecting when sleep starts and ends. Different algorithms are used to classify sleep and wake states based on wrist acceleration data. Deep learning methods have shown potential for precisely identifying sleep stages through accelerometer data. These algorithms leverage various features to enhance the accuracy of sleep detection and staging. When compared to polysomnography, deep learning algorithms perform better in classifying sleep and wake states. Overall, using deep learning with wrist-worn accelerometers represents a promising method for accurately detecting the onset and end of sleep.

**Dataset Overview**

This dataset contains approximately 500 recordings of wrist-worn accelerometer data, spanning multiple days and annotated with two types of events: "onset," marking the start of sleep, and "wakeup," indicating the end of sleep. Your objective is to identify these events within the accelerometer data.

Although sleep logbooks are considered the most accurate method for tracking sleep, in this dataset, sleep is defined as the longest continuous period of inactivity while the watch is worn. Raters have been provided with specific guidelines for annotating the data:

- A sleep period must be at least 30 minutes long.
- A sleep period can be interrupted by periods of activity, as long as these interruptions do not exceed 30 consecutive minutes.
- Sleep windows cannot be recorded unless the watch is confirmed to be worn throughout the duration (details provided below).
- Only the longest sleep period within a night is recorded.
- If no valid sleep window is identified, no onset or wakeup event is recorded for that night.
- Sleep events are not required to span across days, and there is no strict limit on the number of events that can occur in a given period. However, typically only one sleep window should be recorded per night. For instance, it is acceptable for an individual to have sleep periods from 01:00 to 06:00 and from 19:00 to 23:30 on the same calendar day, but these should be assigned to consecutive nights.
- The number of recorded nights is roughly equal to the number of 24-hour periods within the dataset.
- Although each series is continuous, there may be times when the accelerometer was removed, identified by periods of minimal variation in the accelerometer signals over extended durations—an unrealistic scenario for typical human behavior. No events are annotated during these periods, and predictions made during these times will be considered false positives.

Each data series corresponds to a unique experimental subject and represents a continuous recording over multiple days and events.
