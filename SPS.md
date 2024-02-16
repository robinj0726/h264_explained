In H.264, the Sequence Parameter Set (SPS) is a type of non-VCL NAL unit that contains important information about the encoded video sequence. 

The SPS includes parameters that are likely to be the same for a large number of consecutive frames in the video sequence. These parameters are sent relatively infrequently compared to the actual video data, reducing the amount of data that needs to be transmitted.

Here are some of the parameters that the SPS can include:

- Profile indication: Specifies the encoding methods used in the bitstream.
- Level indication: Specifies a set of constraints indicating a degree of required decoder performance for a profile.
- Sequence parameter set ID: Identifies the sequence parameter set.
- Picture order count: Method of determining the display order of the decoded pictures.
- Frame cropping flag: Indicates whether the decoded picture cropping is in use.
- Pixel aspect ratio: Specifies the aspect ratio when it isn't the standard 1:1.
- Frame rate: Information about the frame rate of the video.
- Video resolution: The width and height of the video.

The decoder uses the information in the SPS to correctly decode the video frames. The SPS is usually sent at the start of a video stream and whenever the information it contains changes.