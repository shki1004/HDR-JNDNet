# HDR-JNDNet

Subjective Test videos (4K-UHD/10-bit HDR)
- Link: https://www.dropbox.com/sh/mpmih6xik064j5r/AACLVhxKeWRN1emz32Q7fWGRa?dl=0
- If 4K-UHD/HDR TV is available, you can perform the subjective visual quality comparison

## Explain for test videos
For testing, we use 10 testing 4K-UHD (3840x2160) 10-bit HDR video clips. Test HDR videos are quantized 10-bit YCbCr 4:2:0 format within the BT2020 color container after applying the perceptual quantization (PQ) transfer function. And the test HDR videos are encoded using the HEVC reference software (HM16.17) under the main10 HDR Random-Access profile for 4 QP values of 22, 27, 32, and 37. Since the HDR-JNDNet generates the adjusted ERJND_hdr-directed energy-reduced frames only for Y-channel frames, Cb- and Cr-channel frames of input HDR videos are encoded without preprocessing in our preprocessing-based HDR video coding scheme. In this work, we focused on the energy-reduction of Y-channel because the data sizes of the Cb- and Cr-channel frames are one-fourth of the Y-channel frames in YCbCr 4:2:0 format. 

## Explain for subjective tests
we performed subjective tests to measure the perceptual qualities of decoded HDR videos. The subjective tests were performed under common test conditions. The DSCQS (double stimulus continuous quality scale) method was used for subjective evaluation. Both the reference video and the degraded video were evaluated with subjective voting scores in Mean Opinion Score (MOS), which ranged from 0 to 100 for the worst and the best perceptual qualities, respectively. Then, the two obtained MOS values were converted into a DMOS (Differential Mean Opinion Score) value, which is defined as the MOS value of the reference video minus that of the degraded video, to compare their perceptual quality. The displays used for the subjective tests were an LG 65EF950 4K-UHD/HDR TV for the 4K-UHD/HDR test videos. The viewing distances for 4K-UHD/HDR videos are 1.6H, H is the height of the display. A total of 20 subjects (male: 15, female: 5, average age: 23.25, max-age: 26, min-age: 22) with normal vision who were non-experts in image processing participated in the subjective quality assessment experiments.

## Explain files in folder
In SubjectiveTestVideos folder, There are 4 test videos and 4 text files for 4 QP values (22, 27, 32, and 37). The one subjective test video file is composed to the 20 encoded videos (reference video(without preprocessing) and degraded video(with preprocessing)) for total 10 test 4K-UHD/10-bit HDR videos. And the orders of reference and degraded video are randomly determined. The determined orders are noted in text files.  
