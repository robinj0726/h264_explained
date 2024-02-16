In H.264 (also known as MPEG-4 AVC), NAL stands for Network Abstraction Layer. The NAL is a part of the video codec that handles the encapsulation and representation of data. 

The NAL provides a network-friendly video representation format that abstracts the data in a way that allows it to be sent and received over a variety of networks and systems. 

Each unit of data in this layer is called a NAL unit. NAL units are classified into two types: VCL (Video Coding Layer) NAL units, which contain the actual visual data, and non-VCL NAL units, which contain metadata such as sequence parameters and picture parameters. 

The NAL, along with the Video Coding Layer (VCL), forms the two main parts of the H.264 codec. The VCL is responsible for the efficient representation of the video content, while the NAL formats the VCL representation and provides header information in a way that is appropriate for conveyance by transport layers or storage media.

In H.264, Network Abstraction Layer (NAL) units are categorized into two types: VCL (Video Coding Layer) NAL units and non-VCL NAL units.

1. VCL NAL Units: These contain the actual visual (video) data. They include the coded slices of a picture and are responsible for the efficient representation of the video content.

2. Non-VCL NAL Units: These do not contain encoded picture data but instead carry metadata that is used in the decoding process or for network transport. They include:

   - Sequence Parameter Set (SPS): Contains parameters that apply to a series of consecutive coded video pictures.
   
   - Picture Parameter Set (PPS): Contains parameters that apply to the decoding of one or more individual pictures within a coded video sequence.
   
   - Access Unit Delimiter (AUD): An optional NAL unit that can be used to indicate the boundary of access units.
   
   - End of Sequence (EOS) and End of Stream (EOS): Used to indicate the end of a coded sequence or a coded bitstream.
   
   - Filler Data: Used in certain streaming applications where a constant bit rate is required.
   
   - SEI (Supplemental Enhancement Information): Carries additional information that may be used to enhance the usability of the video payload.

Each NAL unit starts with a header that indicates the type of the NAL unit, which helps the decoder to interpret the content of the NAL unit correctly.