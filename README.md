# Video-based-Person-Re-Identification
One popular video-based Person Re-Identification (ReID) algorithm is the Part-based Convolutional Baseline (PCB) algorithm. This algorithm learns a part-based representation of person images by dividing the image into several horizontal stripes and then training a separate classifier for each stripe. This allows for better localization of body parts and improves ReID performance.

To implement PCB, I would use the PyTorch library and the pre-trained models provided by the authors of PCB on the Market-1501 dataset. I would choose this implementation over others because it has been widely used and has shown good performance on multiple datasets. Additionally, the pre-trained models provided by the authors make it easy to get started and make it replicable.

I would use the following steps:

1. Install PyTorch and torchvision library
2. Download the pre-trained PCB models from the author's website
3. Prepare the video dataset for training and testing by using video frames
4. Create a PCB model by using the pre-trained models and fine-tune it on the dataset
5. Test the model on the test set and evaluate the performance using metrics such as rank-1 accuracy, mAP and CMC
6. Implement the PCB model in real-time by using the webcam or a video file as input, detect and cropping the person bounding box, and output the predicted person ID in real-time.
Compared to traditional trackers like FairMOT or DeepSORT, person Re-ID algorithms like PCB are specifically designed for person re-identification and are typically more robust to occlusions and viewpoint changes. However, traditional trackers like FairMOT and DeepSORT are more appropriate for multi-camera tracking scenarios, where the goal is to track the same person across multiple cameras, whereas Re-ID algorithms are designed to match a person across different camera views.
