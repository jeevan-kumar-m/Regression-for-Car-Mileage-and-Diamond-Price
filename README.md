# Regression-for-Car-Mileage-and-Diamond-Price



## Task 1: Video Processing Pipeline

### Video Ingestion:

This section encompasses the initial step of the video processing pipeline, focusing on the ingestion of a video file. Using the `cv2` library in Python, the script opens the specified video file (`'video.mp4'`). It then iterates through each frame of the video, processing them one by one. This stage is crucial for accessing the raw video data and preparing it for subsequent analysis.

### Frame Processing:

The frame processing stage involves extracting essential information from each frame and saving them for further analysis. As frames are extracted from the video, metadata such as camera ID and geographic location are generated. Additionally, frames are saved as JPEG images to facilitate easier handling and manipulation. This step is essential for extracting meaningful insights from the video data.

### Batching:

Batching involves organizing frames into manageable groups for more efficient processing. The script divides the frames into batches based on a predefined duration specified in the configuration. Each batch represents a specific time interval of the video. This batching process ensures that the processing workload is distributed evenly and allows for better resource management during analysis.

### Data Storage:

In this section, the processed data is stored in a structured format for future reference and analysis. The script utilizes a SQLite database to store information about each batch of frames, including batch ID, start and end frame IDs, and timestamps. This data storage mechanism enables easy retrieval and querying of video processing results, facilitating further analysis and visualization.

### Concurrency and Error Handling:

Concurrency and error handling mechanisms are essential for ensuring the robustness and reliability of the video processing pipeline. The script employs threading to parallelize the processing of video streams, improving overall efficiency. Additionally, error handling mechanisms are implemented to gracefully handle any exceptions or errors that may occur during processing. This ensures that the pipeline can recover from errors and continue processing without interruption.

---

## Task 2: User Input Handling

### Get User Input:

This task involves interacting with the user to obtain input parameters required for the video processing pipeline. Specifically, the script prompts the user to enter a timestamp in a specified format (`YYYY-MM-DD HH:MM:SS`) and a duration in seconds. These input parameters serve as key inputs for configuring the video processing pipeline according to the user's requirements.

---
